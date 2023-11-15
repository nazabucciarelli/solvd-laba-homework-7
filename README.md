# 7th Homework of Java Test Automation Course - Solvd Laba
This repository stores the 7th homework given by our mentor in the Java Test
Automation Course at Solvd Laba. It consists in a modification of the last
homework (6th), now we had to convert the current project in a Maven one,
add two plugins to it and interact with the different phases of the Maven 
lifecycle.

## Explanation

To accomplish the requirements of the homework, I've manually converted the 
project in a Maven project and set the proper configuration for the pom.xml
file, adding the log4j-api and log4j-core as dependencies from there.
After, I've added two plugins: maven-compiler-plugin, that is used to compile 
the sources of the project in the desired version, and maven-surefire-plugin,
that is used for running the unit tests of an application and generate reports.
Finally, I've run the different phases of the Maven lifecycle:
- mvn validate: It validated that the project was correct.
- mvn compile: It compiled the source code and put it into the target folder. It created it automatically.
- mvn test: As I have no tests in the project, it just printed "No tests to run".
- mvn package: It packaged the compiled code in the .jar format and saved it in the target folder.
- mvn verify: It did nothing, because its task is to perform integration tests that maven finds in the project and this project doesn't have any.
- mvn install: It installed the package into the local repository (.m2).
- mvn deploy: It threw an error because I haven't specified any repository in the pom.xml.
By running "mvn package" and "mvn install", the .jar file was created and installed
in the local repository (1st exercise).

## Technologies

- Java
- Maven

## Set-Up

To run this project you will need an updated version of Java.
First, clone this repository in a folder of your PC.
You have to put the following command in a terminal:

```bash
  git clone this-repo-url
```
You will need an IDE to open the project folder and, finally, run the Main.java
file to see the program output.

## Author

- [@Nazareno Bucciarelli](https://github.com/nazabucciarelli)