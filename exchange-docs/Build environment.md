All Mule applications run under the Java Runtime Environment (JRE). Application components are built and deployed using Maven, a popular software management tool used in DevOps environments. MuleSoft also provides an Eclipse-based Integrated Development Environment (IDE) called Anypoint Studio, which is used for developing Mule applications in a graphical environment. While Studio can also be used for building, testing, and deploying applications, the instructions provided in the readme documentation of the projects assume the use of Maven from the command line, except where noted.

## Software Requirements

The MuleSoft Assets are built on Mule 4 and Studio 7. The following is a list of the minimum software requirements for working with Accelerator assets:

* Anypoint Studio 7.12.0 or higher
* Mule Runtime 4.4.0 or higher (included with Studio)
* Latest AdoptOpenJDK 8 release (included with Studio)
* Latest Maven 3.8.x release (for command-line deployments)
* Postman 9.x or higher (for API testing)

## Workstation Setup

Perform the following steps to prepare your workstation for building, deploying, and testing Mulesoft assets. These instructions assume some basic knowledge of using Maven and Eclipse-based products.

## Installing

- Download and install the latest 64-bit version of the OpenJDK 8 release from [https://adoptopenjdk.net](https://adoptopenjdk.net)
   . On Windows, add or update the `JAVA_HOME` environment variable to point to the installation root directory, for example `C:\Program Files\Java\jdk1.8.0_265`, and append `%JAVA_HOME%\bin` to the `PATH` variable.
- Download and install the latest Apache Maven 3.8.x release from [http://maven.apache.org/download.cgi](http://maven.apache.org/download.cgi) . Add or update the `MAVEN_HOME` environment variable to point to the installation root directory, for example `C:\Utilities\apache-maven-3.8.4`, and append `%MAVEN_HOME%\bin` (`$MAVEN_HOME/bin` on Linux/MacOS) to the `PATH` variable.
- Download and install the latest 64-bit version of the Anypoint Studio 7 release from [https://www.mulesoft.com/lp/dl/studio](https://www.mulesoft.com/lp/dl/studio). Do not install the product under a folder containing spaces in the name.
- Launch Studio and create a new workspace for the accelerator assets. Do not locate the workspace under a folder containing spaces in the name.

