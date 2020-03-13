# maven
use all the projects separately

simple-single project:
1. refer this to start with maven
2. consists of single source code

simple-multi project:
1. refer this to start with understanding how multi-module works
2. sub-modules will create jar files

app-multi project:
1. You will learn how to establish a dependency between a web module and a Java library module.
2. use Maven to package the WAR file and the JAR file into an EAR file so that you can run and test the application on Open Liberty.
3. You will build a unit converter application that converts heights from centimeters into feet and inches. Enter heights in centimeters from a web page, and the application processes the input with functions in the JAR file to return the corresponding height in Imperial units.
4. each module has its own pom.xml file because each module is treated as an independent project. You can rebuild, reuse, and reassemble every module on its own.
5. Navigate to the start directory to begin.
 This folder includes a web module in the war folder, a Java library in the jar folder, and template files in the ear folder. However, the Java library and the web module are independent projects, and you will need to complete the following steps to implement the application:
Add a dependency relationship between two modules.
Assemble the entire application into an EAR file.
Aggregate the entire build.
Test the multi-module application.
6. To deploy your EAR application on an Open Liberty server, run the Maven liberty:run goal from the ear directory:
mvn liberty:run
Once the server is running, you can find the application at the following URL: http://localhost:9080/converter/
7. After you are finished checking out the application, stop the Open Liberty server by pressing CTRL+C in the shell session where you ran the server. Alternatively, you can run the liberty:stop goal from the start\ear directory in another shell session:
mvn liberty:stop
