# aem-guide-dependency-installation for AEM 6.5 

# Installing Dependency via  
## Verifying your Version - MAC 
  1. Verify Latest Version of Maven


  ![alt text](https://res.cloudinary.com/ddid7dngp/image/upload/v1666626790/Apache_Maven_3.8.6_84538c9988a25aec085021c365c560670ad80163_l2gwac.jpg "Maven Version Screenshot")
  
  
  2. Verify Java SDK 11


  ![alt text](https://res.cloudinary.com/ddid7dngp/image/upload/v1666627326/Java_version_11.0.16.1_2022-08-18_LTS_sd9b5u.jpg "Java Version Screenshot")

# Installing Maven (3.8.6) and Java 11

## Prerequisite - Homebrew

Homebrew is an free open source package manager that allows you to install and uninstall dependencies. Using homebrew, you will not need to change variables in the bash profile which makes it SUPER convenient. 

To install homebrew click --> [here](https://brew.sh/)

verify homebrew using: 

brew --version

# Installation

1. Go to the terminal and run home brew command: brew install maven

The above code will install the latest version of Maven. This is what we'll need. 

ONLY with homebrew can you install Maven with the above commands.

2. Install Java 11 - Inside the same terminal you will need to run:

brew install java (specify version here)

3. Once both are installed. Run a new terminal and check each version by running:


  java -version


  mvn -v 
  
4. All Done!

---
---



# Windows 


## Installing Java 11


### In order to correctly run an authoring instance of Adobe Experience Manager you must install Java 11

1. Navigate to the [Java SE Downloads](https://www.oracle.com/java/technologies/downloads/#java11-windows) page and scroll down until you see Java 8 and Java 11
2. Click Java 11
3. Select your respective operating system and click the x64 download link for JDK 11
4. You have two options from which to proceed: start the JDK installer by double-clicking the file name in the downloads section || OR ||
  install JDK 11 in slient mode within the command line: `jdk.exe /s`
  
## Set Environmental Variables in Java

### Add Java to System Variables

1. Open the **Start** menu and search for environment variables
2. Select the result: **Edit the system environment variables**
3. In the System Properties window, under the **Advanced** tab, click **Environment Variables**
4. Under the System variables category, select the **Path** variable and click **Edit**
5. Click **New**
6. The default path is typically *C:\Program Files\Java\jdk-11.0.16.1\bin*

*You may find your specific path via File Explorer*

### Add JAVA_HOME Variable

1. Again, in the **Environment Variables** window, select **New** under System variables
2. Input `JAVA_HOME` as the Variable name
3. In the value field, enter the path to your **Java jdk-11** directory *not* the bin 
4. Confirm the changes
 

### Verify Java Instalation
1. Run `java -version` in the command prompt

---
## Installing Maven

### Download Maven Zip File and Extract
1. Navigate to the [Maven Downloads](https://maven.apache.org/download.cgi) page 
2. Select and download the apache-maven **zip** file
3. Maven does not have an installation process... so, simply extract the Maven archive

### Add MAVEN_HOME System Variable

1. Recall how you navigated to the **Environment Variables** windows
2. Once again you will select **New** under System variables
3. Input `MAVEN_HOME` as the Variable name
4. Just as you entered in the path value for Java, you will enter the path value for **Maven**

### Add MAVEN_HOME Directory in PATH Variable
1. Select the **Path** variable under the System variables section
2. Click the **Edit** button and edit the variable
3. Once the Edit environment variable opens, click **New**
4. Input **%MAVEN_HOME%\bin** and save the changes by clicking **OK** in both windows

### Verify Maven Installation

1. Run `mvn -version` in the command line

---
---
Continue with your [AEM training journey](https://github.com/matthew-acn/aem_guide) 
