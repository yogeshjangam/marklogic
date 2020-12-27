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
D. and run below command to setup our first database project 'mlNewProject' using below:

    PS test-ml-gradle> gradle mlNewProject

# todo-yj start here

D. Answer the questions asked in the prompts

    Task :mlNewProject
    Welcome to the new project wizard. Please answer the following questions to start a new project.
    Note that this will overwrite your current build.gradle and gradle.properties files, and backup copies of each will be made.
    [ant:input] Application name: [myApp]
    <-<--<-------------> 0% EXECUTING [7s]
    [ant:input] Host to deploy to: [localhost]
    <-------<-------------> 0% EXECUTING [12s]
    [ant:input] MarkLogic admin username: [admin]
    <----<-------------> 0% EXECUTING [15s]
    [ant:input] MarkLogic admin password: [admin]
    <-<-------------> 0% EXECUTING [26s]
    [ant:input] REST API port (leave blank for no REST API server):
    <<<-------------> 0% EXECUTING [34s]
    [ant:input] Test REST API port (intended for running automated tests; leave blank for no server):
    <---<-------------> 0% EXECUTING [42s]
    [ant:input] Do you want support for multiple environments?  ([y], n)
    <<-------------> 0% EXECUTING [47s]
    [ant:input] Do you want resource files for a content database and set of users/roles created? ([y], n)
    <-------------> 0% EXECUTING [54s]
    Writing: gradle.properties
    Making directory: \test-ml-gradle\src\main\ml-config
    Making directory: \test-ml-gradle\src\main\ml-modules
    Writing project scaffolding files

Once that is done run

    gradle mlDeploy
