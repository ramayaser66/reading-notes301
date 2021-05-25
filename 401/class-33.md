

##  Review of Serverless 

Serverless computing is a method of providing backend services on an as-used basis. Servers are still used, but a company that gets backend services from a serverless vendor is charged based on usage, not a fixed amount of bandwidth or number of servers.



## AWS Amplify 
AWS Amplify is a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications, powered by AWS.

Amplify libraries support iOS, Android, Web, Flutter, and React Native apps. For Web apps, there is deep integration with React, Ionic, Angular, and Vue. js.



## API (GRAPHQL) 

**Add relationships between types**
`@connection`

 enables you to specify relationships between @model types --> 

-  one-to-one 
-  one-to-many
- many-to-one  

Note:  You may implement many-to-many relationships using two one-to-many connections and a joining @model type. 

**Usage**

`fields` argument can be provided and indicates which fields can be queried by to get connected objects.

`keyName` argument can optionally be used to specify the name of secondary index (an index that was set up using @key) that should be queried from the other type in the relationship. 

`Has one` 
`Has many`
`Belongs to`

Note:  connection bi-directional by adding a many-to-one connection to types that already have a one-to-many connection.

`Many-to-many connections`