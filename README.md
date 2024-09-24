# maven-multi-module-template

## Examples of usage

## spring boot multi module

1) in every module use the same package namespace
    For example: everywhere the namespace: be.fve.personalprojects
2) use name convention correctly:
    - be-fve-project-api
        -  this is for all endpoints and restcontroller etc.
    - be-fve-project-dao
        - this is for everything JPA and DB and repository related
    - be-fve-project-packaging
        - this is where the spring-boot-maven-plugin exists and where the jar is being built for the full program
    - be-fve-project-model
        - here are all the model classes that are standalone without relation to DB or so
    - be-fve-project-utils
        - all custom standalone functions reusable are in here
    - be-fve-project-testutils
        - everything for testing such as custom classes, annotations, configuration, dependencies etc. are in here
    - be-fve-springbootstarter-...
        - this are standalone spring boot starter libraries to be used in the project
    - be-fve-lib-...
        - these are standalone java libraries to be used in java projects
    - be-fve-project-clients
        - this is for consuming external clients and to connect with
    - be-fve-project-service
        - all services in the project are in here
    - be-fve-project-facade
        - all classes facade related to connect modules are in here
    - be-fve-project-application
        - all configuration and setup for initialization of the application happens in here, like the application.yml etc.

3) op root niveau zet je de docker-compose.yml,  gitignore file, lombok.config, etc.
    
