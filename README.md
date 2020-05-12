# Archetype
This project provides a maven project archetype which uses the following structure:

```
pom.xml
README.MD
src
└──main
│    └──java
│    │    └──ar
│    │        └──com
│    │            └──wolox
│    │                └──api
│    │                    └──controllers
│    │                    └──dtos
│    │                    └──exceptions
│    │                    └──models
│    │                    └──repositories
│    │                    └──repositories
│    │                    └──services
│    │                    └──utils
|    |                      Application.Java
│    └──resources
│           application.properties
└──test
     └──java
     │    └──ar
     │        └──com
     │            └──wolox
     │                └──api
     |                      ApplicationTests.Java
     └──resources
            application.properties
```

The dependencies from this archetype are:

- spring-boot-starter-parent 2.2.6 (*Parent*)
- spring-boot-starter
- spring-boot-starter-data-jpa
- spring-boot-starter-security
- spring-boot-starter-test
- spring-security-test
- org.postgresql
- com.h2database
- spring-boot-starter-web
- com.google.guava 27.0
- org.modelmapper 2.3.3


Ones this project is imported from git, you can install it with `mvn install` to have it in your own local 
repository.

Then, to create a project following this archetype run this command (Setting the needed variables): 

```
mvn archetype:generate 
    -DarchetypeGroupId=ar.com.wolox 
    -DarchetypeArtifactId=wolox-archetype
    -DarchetypeVersion=1.0
    -DgroupId={YOUR_GROUP_ID}
    -DartifactId={YOUR_PROJECT_ID}
    -Dversion={YOUR_PROJECT_VERSION}
```
