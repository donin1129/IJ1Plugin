# About this project

This project is meant to serve as an example how to write plugin for ij1 and fiji using Gradle Kotlin build system in a modern IDE such as IntelliJ.

The example using Maven build can be found https://github.com/imagej/example-legacy-plugin. 

## How to work with this?

### 1. Install JDK
You have to work with Java SE version equal or earlier than Java 8. Therefore, you need to use JDK such as from https://adoptium.net/temurin/releases/?variant=openjdk8.

You can also install another JDK of your choice to see if it works.

### 2. Build jar

Use command ```.\gradlew build```
Or use IDE convenient tools to build jar.

### 3. Copy jar from build location to plugins directory

After the build, a file will be generated at `./build/libs/IJPluginGradle-1.0.jar`.
Copy this file and add it to imagej plugins directory. For Fiji, it should be located at `./Fiji.app/plugins`.

### 4. Start imagej

You should be able to find the plugin at `Process | Process Pixels`.

## System Considerations

* I have **Windows 10 Pro** but any Windows system should work with this project. (Not sure how it will behave on a Unix)
* I am using JDK temurin-1.8 from https://adoptium.net/temurin/releases/?version=8&package=jdk&arch=x64&os=windows. 