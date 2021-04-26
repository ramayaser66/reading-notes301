
# Hibernate relationships

## @ManyToMany annotation 

![](https://www.baeldung.com/wp-content/uploads/2018/11/relation-attribute-model-updated.png)
_______________________________________________________
Hibernate many to many mapping is made between two entities where one can have relation with multiple other entity instances.

@ManyToMany annotation is used in both classes to create the many-to-many relationship between the entities. 

- Database Setup 
you will need to create a Data base with tables for the entities in the many to many relation.

 you will need the suitable dependencies and Hibernate configuration.

 any model class needs to be created with JPA annotation 

 classes will refer to one another, which means that the association between them is bidirectional.


 In order to map a many-to-many association we use: @ManyToMany annotations
 @JoinTable  annotations
 @JoinColumn  annotations

 mappedBy attribute is used in the @ManyToMany annotation to indicate that the first model collection  is mapped by the second model collection of the owner side
 

![](http://norows.com/wp-content/uploads/2018/05/relationships.png)




