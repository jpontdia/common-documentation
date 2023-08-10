# Documentation - Build Environment
Mulesoft Documentation - Development -  Build environment

## Configure group-id of the project

In order to deploy the asset in your Anypoint Exchange you must set the business group of your organization in the pom.xml file in the section groupId, example:

```xml 
    <groupId>my-business-group-id</groupId>
```

## Exchange deployment
maven command to deploy asset in anypoint exchange:

```bash 
mvn deploy
```