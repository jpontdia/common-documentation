# Documentation - Development Process
Mulesoft Documentation - Development Process

## Configure group-id of the project

In order to deploy the documentation in your Anypoint Exchange you must set the business group of your organization in the pom.xml file in the section groupId, example:

```xml 
    <groupId>my-business-group-id</groupId>
```

## Exchange deployment
maven command to deploy asset in anypoint exchange:

```bash 
mvn deploy
```