# JAVA-MAVEN-VSCODE

Test example to set a java maven project with selenium in VS Code

## Table of Contents

- [JAVA-MAVEN-VSCODE](#java-maven-vscode)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)

## Installation

* Download JDK
* brew install maven
  * java version "21.0.2" 2024-01-16 LTS
  * Java(TM) SE Runtime Environment (build 21.0.2+13-LTS-58)
  * Java HotSpot(TM) 64-Bit Server VM (build 21.0.2+13-LTS-58, mixed mode, sharing)
* Download chrome driver
  * https://googlechromelabs.github.io/chrome-for-testing/

* Cmd + shift + P -> maven project 
* Maven archetype quickstart -> it creates a folder “demo” (it can be changed, this will be the name of the project folder)
* Add selenium dependency

```xml
<dependency>
      <groupId>org.seleniumhq.selenium</groupId>
      <artifactId>selenium-java</artifactId>
      <version>3.141.59</version>
 </dependency>
```
* mvn clean install (to check everything is ok)

* Note: sometimes chomedriver in chrome is not detected in mac, so run this command in the path where the chromedriver is stored

```
xattr -d com.apple.quarantine chromedriver
```
