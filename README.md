# drivers.gradle for Katalon Studio
## What is this?

This project provides a set of files which is supposed to be copied and pasted
into your own [Katalon Studio](https://www.katalon.com/) projects.
A [Gradle](https://gradle.org/) build file named `drivers.gradle` is included.
Also the files called [Gradle wrapper](https://docs.gradle.org/current/userguide/gradle_wrapper.html) is included.
You can execute `drivers.gradle` with Gradle Wrapper. By doing so, you can download
specified version of external jar files from public sites and locate them into the `Drivers` folder of your projects. Gradle build script with Gradle Wrapper is convenient, easily repeatable, fail-safe way of managing jars.

## Problem to solve

Katalon Studio allows users to use external Java .jar libraries as described
in the official document
[External Libraries](https://docs.katalon.com/katalon-studio/docs/external-libraries.html).

For example, I often want to use the AShot library distributed at the Maven Centroal Repository:
- https://mvnrepository.com/artifact/ru.yandex.qatools.ashot/ashot/1.5.4

Also I often want to use the Materials library which I developed. The Materials library is
published at Github Releases page:
- https://github.com/kazurayam/Materials/releases

When I create a new Katalon Studio project, of course, I can manually download the jar files
and place them into the `Drivers` folder. Though it is easy enough but I wanted to automate it by Gradle build script. I had 2 reasons.

Reason 1:

Reason 2:

## How to utilize drivers.gradle

### Prerequisite

```
C:\Users\myname> java -version
java version "1.8.0_191"
Java(TM) SE Runtime Environment (build 1.8.0_191-b12)
Java HostSpot(TM) 64-Bit Server VM (build 25.191-b12, mixed mode)
```

[Java SE Development Kit 8 Downloads](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
