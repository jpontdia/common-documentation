## Table of contents
1. [Documentation](#documentation)
1. [Configuration](#configuration)

## Documentation

### Readme.md as one source for documentation

The documentation for the code repository is used in Anypoint Exchange as one source of truth. The file README.md in the project's root is used to store the documentation for the mule application; any other resource (documents, images, etc.) referenced by the readme file will be stored in the docs directory.

The CICD pipeline will copy the README.md file and docs directory into the exchange-docs directory.

The maven exchange-mule-maven-plugin will be responsible for packaging the contents of the exchange-docs directory and publishing it along with the asset in Anypoint Exchange. The Maven plugin is configured in the parent-pom used by the project. The developer is only accountable for generating accurate and meaningful documentation for the project in one REAME.md file.

Guidelines:
- Use one README.md file. Although GitHub and Anypoint Exchange can present multiple documents, We will use only one to simplify the documentation and packaging process.
- In the README.md, use the following syntax to reference an image or file in the docs directory: docs/myfile.png. 

### Document structure

The README.md file will have at least the following sections:

1. Name of the project.
1. Code Badges.
1. A short description of the project, the same one used in the description of the code repository.
1. Legend: This project follows the standards defined in the Development Process Document in Anypoint Exchange. The details about how to compile and package the asset are in the Build Environemnt section. 
1. Table of contents.
1. Description: Detail documentation about the service: objectives, functionality, architecture diagrams, etc. This section can be split into multiple sub-sections to improve the readability and organization of the information.
1. Configuration: Explanation of all the parameters used by the application.

Suppose the project has different prerequisites for compilation than those expressed in the build environment guide, or the packaging procedure is not standard. In that case, a new section must be added explaining the differences.

## Configuration

The configuration follows the principles of [12 Factor apps](https://12factor.net/config). The configuration of the application is handled in the CICD pipeline.

### Configuration file
The configuration file for the project is: /src/main/resources/config.yaml. Prohibited the use of secure configuration files or configuration file per environment, example: config-prd.yaml
