## Set up your local development environment

### ⏱ 10 min read

MessageBird provides an SDK (Software Development Kit) for Java. This helper library facilitates interactions between your Java application's code and the MessageBird APIs, so you do not have to craft raw REST API requests.

This MessageBird Developer Tutorial explains how to get started with MessageBird in Java by first setting up your local development environment.

## Install Java and Maven

You should make sure that you have at least Java version 1.5 installed on your computer, as this is the minimum version of Java that the SDK requires. You also need Maven, a package manager for Java. It's recommended that you always use the latest versions of Java and Maven.

To verify, open a terminal and run the following two commands:

```
java --version
mvn --version
```

In both cases, your terminal should return a version number, like this:

```
$ java --version
openjdk 11 2018-09-25
OpenJDK Runtime Environment 18.9 (build 11+28)
OpenJDK 64-Bit Server VM 18.9 (build 11+28, mixed mode)
$ mvn --version
Apache Maven 3.0.5 (...)
Maven home: ...
Java version: 1.8.0_60, vendor: Oracle Corporation
Java home: ...
Default locale: en_US, platform encoding: Cp1252
OS name: "windows 7", version: "6.1", arch: "amd64", family: "dos"
```

If you do not get a version number but something like `java: command not found` instead, you need to install Java and Maven first.

Follow the instructions on the [Java 1.8](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html), which will provide more guidance on installing Java for your operating system.

## Install the MessageBird SDK

You use Maven to install the MessageBird SDK for Java. The SDK is open source and you can [browse the code in this GitHub repository](https://github.com/messagebird/java-rest-api). It is also [listed on the Maven repository website](https://mvnrepository.com/artifact/com.messagebird/messagebird-api) so that Maven knows where to find it. SDKs and other libraries are always installed for each project as a dependency.

Each Java project that uses Maven needs a `pom.xml` file that includes information both about the current package, i.e., your project, such as name and version, as well as the list of dependencies that it relies on, such as the MessageBird SDK.

Create a new project directory or open an existing project directory in your terminal. 

Once you have a `pom.xml` file, add the `dependency` block to `dependencies` to have Maven install the package:

```xml
<dependencies>
    <dependency>
        <groupId>com.messagebird</groupId>
        <artifactId>messagebird-api</artifactId>
        <version>2.0.0</version>
    </dependency>
</dependencies>
```

## You're ready!

Your Java development environment and project directory are ready now. Let's head over to the next MessageBird Developer Tutorials and [learn how to send your first SMS using Java](https://developers.messagebird.com/tutorials/send-sms).
