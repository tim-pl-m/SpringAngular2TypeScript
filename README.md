[![Build Status](https://travis-ci.org/marco76/SpringAngular2TypeScript.svg?branch=master)](https://travis-ci.org/marco76/SpringAngular2TypeScript) [![star this repo](http://githubbadges.com/star.svg?user=marco76&repo=SpringAngular2TypeScript&style=default)](https://github.com/marco76/SpringAngular2TypeScript)
[![fork this repo](http://githubbadges.com/fork.svg?user=marco76&repo=SpringAngular2TypeScript&style=default)](https://github.com/marco76/SpringAngular2TypeScript/fork)

# SpringAngular2TypeScript

This is an example of implementation of a 'Full Stack Web Application'.
Please note that this code is very experimental and regularly modified.

You can find the running app (deployed via docker) here: http://angular.cafe

Information about the development of this example in the blog here: http://javaee.ch

Stack:
- Spring Boot on the backend
- AngularJS 2 on the frontend
- TypeScript as frontend language
- packaging optimized by webpack

Prerequisites:
- install maven and npm

####For development (js server + java server):
1. Package the java project or launch Application.java from your IDE
 * mvn clean package
2. launch the backend spring boot application, it runs in localhost:8082
    * java -jar [PARENT_MODULE]/server/target/server-0.14-SNAPSHOT.war
3. launch the webpack server for the frontend
    * cd [PARENT_MODULE]/webClient/src
    * npm start
4. go on http://localhost:8080

#####For production (only one war, Javascript souces optimized):
1. in the parent project directory execute
    * mvn clean package
2. launch the backend spring boot application, it runs in localhost:8082
    * java -jar [PARENT_MODULE]/server/target/server-0.14-SNAPSHOT.war
3. open your browser and visit http://localhost:8082

Docker:

build with:
docker build -t my-java-app .
run with:
docker run –rm -it -p 8080:8080  my-java-app java -jar /usr/src/myapp/angular2.jar




















