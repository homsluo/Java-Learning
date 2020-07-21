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
