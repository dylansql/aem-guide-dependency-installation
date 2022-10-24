# aem-guide-dependency-installation for AEM 6.5 

# Verifying your Version - MAC
  1. Verify Latest Version of Maven


  ![alt text](https://res.cloudinary.com/ddid7dngp/image/upload/v1666626790/Apache_Maven_3.8.6_84538c9988a25aec085021c365c560670ad80163_l2gwac.jpg "Maven Version Screenshot")
  
  
  2. Verify Java SDK 11


  ![alt text](https://res.cloudinary.com/ddid7dngp/image/upload/v1666627326/Java_version_11.0.16.1_2022-08-18_LTS_sd9b5u.jpg "Java Version Screenshot")

# Installing Maven (3.8.6) and Java 

Prerequisite - Homebrew

Homebrew is an free open source package manager that allows you to install and uninstall dependencies. Using homebrew, you will not need to change variables in the bash profile which makes it SUPER convenient. 

To install homebrew click --> [here](https://brew.sh/)

verify homebrew using: 

brew --version

1. Go to the terminal and run home brew command: brew install maven

The above code will install the latest version of Maven. This is what we'll need. 

ONLY with homebrew can you install Maven with the above commands.

2. Install Java 11 - Inside the same terminal you will need to run:

brew install java (specify version here)

3. Once both are installed. Run a new terminal and check each version by running:


java -version


mvn -v 


