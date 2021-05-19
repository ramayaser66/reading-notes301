

# Room in Android 

## Save data in a local database using Room 

importance: 
 structured data can be presented locally. 
 caching relevant pieces of data so that when the device cannot access the network, the user can still browse that content while they are offline.

 advantages of using the room presistane library: 

- it provides an abstraction layer over SQLite to allow fluent database access. 

 - Compile-time verification of SQL queries.
- Convenience annotations that minimize repetitive and error-prone boilerplate code.
- Streamlined database migration paths.

to be able to use a room in the app you'll need to use  the right dependencie, 

`dependencies {
    def room_version = "2.3.0"
    implementation "androidx.room:room-runtime:$room_version"
    annotationProcessor "androidx.room:room-compiler:$room_version"}`



## room components: 

- `database class `

the main access point for the underlying connection to your app's persisted data.

it provides your app with instances of the DAOs associated with that database

- `Data entities `
represent tables in your app's database.

 you define entities to represent the objects that you want to store. Each entity corresponds to a table in the associated Room database,





-` Data access objects (DAOs) `
provide methods that your app can use to query,
   update,
   insert,
   and delete data in the database. 

   the app can use the DAOs to retrieve data from the database as instances of the associated data entity objects. 

    it can use the defined data entities to update rows from the corresponding tables, or to create new rows for insertion. 


## implementing  a room 

1. Data entity 
annotate the class with 
`@Enitiy ` and start working on your table 
Each instance of the model represents a row in a class table in the app's database.

Note:
-  Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table. The most straightforward way of doing this is to annotate a single column with @PrimaryKey

-  composite primary key 
If you need instances of an entity to be uniquely identified by a combination of multiple columns,
example, 
`@Entity(primaryKeys = {"firstName", "lastName"})`

- Ignore fields 
 If an entity has fields that you don't want to persist, you can annotate them using @Ignore 



2. Data access object (DAO) 
`@Dao` 

modelDao provides the methods that the rest of the app uses to interact with data in the model table.

like, 
` @Query("SELECT * FROM user")`

`  @Query("SELECT * FROM user WHERE uid IN (:userIds)")`

` @Query("SELECT * FROM user WHERE first_name LIKE :first AND " +
           "last_name LIKE :last LIMIT 1")`


## Database 

an AppDatabase class holds the database.

 defines the database configuration and serves as the app's main access point to the persisted data. 

 following these conditions:

 - The class must be annotated with a @Database annotation that includes an entities array that lists all of the data entities associated with the database 

- The class must be an abstract class that extends RoomDatabase. 

- For each DAO class that is associated with the database, the database class must define an abstract method that has zero arguments and returns an instance of the DAO class.
Kotlin 

## relationships between objects 

most object-relational mapping libraries allow entity objects to reference each other, Room explicitly forbids it. 

### Create embedded objects 

use the @Embedded annotation to represent an object that you'd like to decompose into its subfields within a table.


- ##  one-to-one relationships 

each instance of the parent entity corresponds to exactly one instance of the child entity

- ##  one-to-many relationships 

a relationship where each instance of the parent entity corresponds to zero or more instances of the child entity, but each instance of the child entity can only correspond to exactly one instance of the parent entity.

- ##  many-to-many relationships 

a relationship where each instance of the parent entity corresponds to zero or more instances of the child entity.

- ## nested relationships 

when you need to query a set of three or more tables that are all related to each other, you define nested relationships between the tables. 


## Accessing data using Room DAOs 

as mentioned before you interact with the stored data by defining data access objects, 

you use  DAOs to access your app's database instead of query builders or direct queries. 


## Anatomy of a DAO

-  each DAO as either an interface or an abstract class, it  usually an interface.

- annotate your DAOs with @Dao 

- types of DAO methods: 
1. Convenience methods that let you insert, update, and delete rows in your database without writing any SQL code.

      **insert**
      `@Insert` annotation allows you to define methods that insert their parameters into the appropriate table in the database.


      **Update**
      ` @Update` annotation allows you to define methods that update specific rows in a database table. Similarly to `@Insert` methods, @Update methods accept data entity instances as parameters. 

       **Delete**
    ` @Delete` annotation allows you to define methods that delete specific rows from a database table

    
2. Query methods that let you write your own SQL query to interact with the database.

       **Query methods**
   @Query annotation allows you to write SQL statements and expose them as DAO methods. 






