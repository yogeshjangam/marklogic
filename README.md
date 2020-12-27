# Learning MarkLogic 10

## start by installing MarkLogic 10

## then by installing ml-gradle

Installed JDK and MarkLogic 8 or above.
I have installed JDK 13 and ML 10 as on Nov 22, 2019

    PS > java --version

    java 13.0.1 2019-10-15
    Java(TM) SE Runtime Environment (build 13.0.1+9)
    Java HotSpot(TM) 64-Bit Server VM (build 13.0.1+9, mixed mode, sharing)

and gradle

    PS > gradle -v

    Welcome to Gradle 6.0.1!

This would now be used to setup database and code using automation
Once gradle is setup , create a test folder say 'test-ml-gradle for our test proejct that we want to create using ml-gradle

    PS test-ml-gradle> gradle mlNewProject

Answer the questions asked in the prompts

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
