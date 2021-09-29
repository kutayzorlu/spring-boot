# Spring Boot + Spring data JPA + PostgreSQL example

Article link : https://kutayzorlu.com/projects-and-programs/spring-boot-projects


### Repository configuration changes 

    logging.level.org.springframework=INFO
    logging.level.com.mkyong=INFO
    logging.level.com.zaxxer=DEBUG
    logging.level.root=ERROR

    spring.datasource.hikari.connectionTimeout=20000
    spring.datasource.hikari.maximumPoolSize=5

    logging.pattern.console=%-5level %logger{36} - %msg%n

    ## PostgreSQL
    spring.datasource.url=jdbc:postgresql://1.1.1.1:5432/kutayzorlu_com
    spring.datasource.username=kutayzorlu
    spring.datasource.password=kutayzorlu

    ## Show sql commandline  
    spring.jpa.show-sql=true    
      

#### Auto configuration of Table Creation and Validation
    #drop n create table again, good for testing, comment this in production
    spring.jpa.hibernate.ddl-auto=none

    #validate: validate the schema, makes no changes to the database.
    #update: update the schema.
    #create: creates the schema, destroying previous data.
    #create-drop: drop the schema when the SessionFactory is closed explicitly, typically when the application is stopped.
    #none: does nothing with the schema, makes no changes to the database


