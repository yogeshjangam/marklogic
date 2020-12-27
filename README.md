# Learning MarkLogic 10 (updated for version 10.0-15.2 Nov 2020 )

MarkLogic is a multi-modal NoSQL database that helps you store XML, JSON, plain text, geospatial, sematic triples in one single location.  

## Installing MarkLogic 10

1. Download MarkLogic Server from <https://developer.marklogic.com/products/marklogic-server>  
2. Perform typical install as per your OS (I am using Windows 64-bit) <https://docs.marklogic.com/guide/installation>
3. Start the MarkLogic service
4. Visit <http://localhost:8001> and do a typical setup

We would be using ml-gradle next to setup our first database.

## Installing ml-gradle

A. Install latest OpenJDK from <https://jdk.java.net>

    PS> java --version
    openjdk 15.0.1 2020-10-20

B. Install Gradle from <https://gradle.org/releases/>

    PS > gradle -v
    -----------------------------------------------------
    Gradle 6.7.1

C. Create a blank folder called 'test-ml-gradle'
E. Create a blank file called "buid.gradle" and add below lines

    plugins { id "com.marklogic.ml-gradle" version "4.1.1" }
F. and run below command to setup our first database project 'mlNewProject' using below:

    PS test-ml-gradle> gradle mlNewProject

D. This starts the gradle build for ML-GRADLE and presents with you below setup questions that you can update. Ensure you give an rest REST API port number

    Writing: build.gradle
    Writing: gradle.properties
    Writing: gradle-dev.properties
    Writing: gradle-local.properties
    Writing: gradle-qa.properties
    Writing: gradle-prod.properties
    Making directory: test-ml-gradle\src\main\ml-config
    Making directory: \test-ml-gradle\src\main\ml-modules
    Writing project scaffolding files

E. With the gradle config now created, start deploy
    PS> gradle mlDeploy


This creates 3 databases(content,test-content and modules), 2 app servers (app and app test).