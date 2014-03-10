Maven Archetypes
========================

#Description
This project helps to create a multi-module maven project. It contains the following archetype.  
1. parent -- This is the parent project, it also creates a common module in the root parent.   
2. exectable-jar -- this is a submodule which creates fat executable jar.
3. restful-api -- restful api archetype with spring boot and spring mvc
4. webapp -- web application with spring mvc
5. couchdb-design -- create couchdb design doc with couchdbapp. 
6. code quality definition files -- configuration for various code quality tools      

#The following plugin and frameworks are pre configure. 
-  Spring Boot   
-  jacoco   
-  findbug   
-  testng   
-  equalsverifier  
-  mockito  
-  checkers-quals  
-  checkstyle   
-  enforcer   
-  pmd   
-  cobertura    
-  antrun   
-  pojomatic   
-  spring test framework   
 
#Usage 
maven repository: https://github.com/DGHLJ/pub-maven-archetypes/blob/master/

##parent project:
mvn archetype:generate -DarchetypeRepository=https://github.com/DGHLJ/pub-maven-archetypes-repo/raw/master/releases 	-DarchetypeGroupId=com.archetype -DarchetypeArtifactId=mvn-archetype-parent -DarchetypeVersion=1.0 -DgroupId=<project group id> -DartifactId=&lt;project artifact Id&gt;

##executable-jar: 
mvn archetype:generate -DarchetypeRepository=https://github.com/DGHLJ/pub-maven-archetypes-repo/raw/master/releases -DarchetypeGroupId=com.archetype -DarchetypeArtifactId=executable-jar -DarchetypeVersion=1.0 -DgroupId=<submodule group id> -DartifactId=&lt;submodule artifact Id&gt;

##jpa:
mvn archetype:generate -DarchetypeRepository=https://github.com/DGHLJ/pub-maven-archetypes-repo/raw/master/releases -DarchetypeGroupId=com.archetype -DarchetypeArtifactId=jpa -DarchetypeVersion=1.0 -DgroupId=<submodule group id> -DartifactId=&lt;submodule artifact Id&gt;

##restful API
mvn archetype:generate -DarchetypeRepository=https://github.com/DGHLJ/pub-maven-archetypes-repo/raw/master/releases -DarchetypeGroupId=com.archetype -DarchetypeArtifactId=restful-service -DarchetypeVersion=1.0 -DgroupId=<submodule group id> -DartifactId=&lt;submodule artifact Id&gt;

