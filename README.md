# Bootcamp #01 Qualiters club 
Testes de API do manual a CI/CDserverRestAPI

## What is it

This repository was created for the Rest API Testing bootcamp.

## Technologies used

- Postman Desktop
- Node.js v22.4.0
- Newman 6.2.1
- Newman-reporter-html

## Documentation

- Doc da API: [Consult Swagger](https://serverest.dev/)

## How to install the environment

- First: install Node on your computer [download here](https://nodejs.org/en/download/package-manager)

- Second: install Newman globally [download the dependency here](https://www.npmjs.com/package/newman)

```
npm install -g newman
```

- Third: install the reporting dependency (optional) [newman-reporter-html](https://www.npmjs.com/package/newman-reporter-html)

```
npm install -g newman-reporter-html
```
## How to run the tests

### By Postman web or desktop
- Import the collection and the environment
- Run the tests manually or automatically


### By Newman
- Open your preferred console
- Run the following command line to run the tests
````
newman run ServerRest.postman_collection.json -e ServerRest_env.postman_environment.json -r cli

````
- Run tests with report
````
newman run ServerRest.postman_collection.json -e ServerRest_env.postman_environment.json -r cli,htmlextra
````

### Report

If you chose to run the tests with the htmlextra report, you generated an HTML file with the test results, and to check the validations you can open the newman folder that was created in the location where the collection and environment files are.



## Contact
email: ed.charana.pt@gmail.com

