# Documentation - Development Process
![Powered by](https://img.shields.io/badge/Powered%20by-Mulesoft-blue.svg)
  ![Build and deploy](https://github.com/jpontdia/mule-common-documentation/actions/workflows/build.yml/badge.svg)
<br>

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

## Further reading
- Publish Assets Using Maven - https://docs.mulesoft.com/exchange/to-publish-assets-maven

- Exchange documentation examples - https://github.com/mulesoft-labs/exchange-documentation-samples

