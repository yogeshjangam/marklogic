# Things to do

start by installing ml-gradle
    needs JDK and MarkLogic 8 or above. I have installed JDK 13 and ML 10 as on Nov 22

        java 13.0.1 2019-10-15
        Java(TM) SE Runtime Environment (build 13.0.1+9)
        Java HotSpot(TM) 64-Bit Server VM (build 13.0.1+9, mixed mode, sharing)
    Gradle 6
        https://gradle.org/next-steps/?version=6.0.1&format=all

        PS > java --version
java 13.0.1 2019-10-15
Java(TM) SE Runtime Environment (build 13.0.1+9)
Java HotSpot(TM) 64-Bit Server VM (build 13.0.1+9, mixed mode, sharing)

PS > gradle -v

Welcome to Gradle 6.0.1!

Here are the highlights of this release:
 - Substantial improvements in dependency management, including
   - Publishing Gradle Module Metadata in addition to pom.xml
   - Advanced control of transitive versions
   - Support for optional features and dependencies
   - Rules to tweak published metadata
 - Support for Java 13
 - Faster incremental Java and Groovy compilation
 - New Zinc compiler for Scala
 - VS2019 support
 - Support for Gradle Enterprise plugin 3.0

For more details see https://docs.gradle.org/6.0.1/release-notes.html


------------------------------------------------------------
Gradle 6.0.1
------------------------------------------------------------

Build time:   2019-11-18 20:25:01 UTC
Revision:     fad121066a68c4701acd362daf4287a7c309a0f5

Kotlin:       1.3.50
Groovy:       2.5.8
Ant:          Apache Ant(TM) version 1.10.7 compiled on September 1 2019
JVM:          13.0.1 (Oracle Corporation 13.0.1+9)
OS:           Windows 10 10.0 amd64

so we can setup database and code using automation


==================


once gradel is setup
 we run below to  setup a test proejct

 PS C:\yj\src\marklogic\test-ml-gradle> gradle mlNewProject

> Task :mlNewProject
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
Making directory: C:\YJ\src\marklogic\test-ml-gradle\src\main\ml-config
Making directory: C:\YJ\src\marklogic\test-ml-gradle\src\main\ml-modules
Writing project scaffolding files

Deprecated Gradle features were used in this build, making it incompatible with Gradle 7.0.
Use '--warning-mode all' to show the individual deprecation warnings.
See https://docs.gradle.org/6.0.1/userguide/command_line_interface.html#sec:command_line_warnings