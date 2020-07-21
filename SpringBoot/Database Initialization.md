# Database Initialization

```
Types of SQL Languages:
1. DDL: Data Definition Language(CREATE, DROP...)
2. DML: Data Manipulation Language(SELECT, INSERT...)
3. DCL: Data Control Language(GRANT, REVOKE)
4. TCL: Transaction Control Language(SAVEPOINT, ROLLBACK, SET TRANSACTION)
```

## Initialize Using JPA
- JPA has features for DDL generation through two external properties:  
  ```spring.jpa.generate-ddl``` (boolean) switches the feature on and off.  
  ```spring.jpa.hibernate.ddl-auto```(enum) is a Hibernate feature that controls the behavior in a more  
  fine-grained way.
  
## Initialize Using Hibernate
```spring.jpa.hibernate.ddl-auto``` can have ```none```, ```validate```, ```update```, ```create-drop``` values.  
Based on your database is embedded or not(```hsqldb```,```h2```,```derby``` are embedded).

## Initialize Using Spring JDBC
- Spring JDBC has a ```DataSource``` initializer feature.  
  + Spring Boot enables it by default and loads SQL from the standard locations:  
    ```schema.sql``` and ```data.sql``` (in the root of the classpath).
  + In addition Spring Boot will load the ```schema-${platform}.sql``` and ```data-${platform}.sql``` files (if present),  
    where ```platform``` is the value of ```spring.datasource.platform```(e.g. ```hsqldb```, ```h2```, ```oracle```, ```mysql```, ```postgresql```)
