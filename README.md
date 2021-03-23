## PLIR-Dockerized-Setup
1. start openmrs , openhim and hapi-fhir containers  

       `docker-compose up`

    Login with the credentaials below  
* OpenMRS -  http://localhost:8080/openmrs  `admin:Admin123`  
* OpenHIM - http://localhost:9000   `root@openhim.org : openhim-password`   
* Hapi FHir - http://localhost:8090   `hapi:hapi123 ` 

2. Log in to openhim and import the config file at `config/openhim-config.json`

3. start the pipeline

       `docker-compose -f pipeline-compose.yml up`
