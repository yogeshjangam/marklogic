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