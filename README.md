# API Test
Rest API testing from manual to CI/CD

## What is it?
This repository was created for Rest API testing.

## Technology
- Postman
- node version v18.17.0
- Newman version v6.0.0
- Newman-reporter-html

## Documentation
- Technical analysis: 
- Doc API: [Consulte Swagger](https://serverest.dev/#/Usu%C3%A1rios/put_usuarios___id_)
  
## How to install the environment 

- First: install node on your computer [download here](https://nodejs.org/en/download)
- Second: install newman globally [download the dependency here](https://www.npmjs.com/package/newman)
```
npm install -g newman
```
- Third: install the reporting dependency (opcional) [newman-reporter-html](https://www.npmjs.com/package/newman-reporter-html)

## How to run the tests

### Postman web or desktop
-Import the collection and environment
-Execute tests manually or automated

### Newman
- Open the console and run the following command line to run the tests
```
newman run ServeRest.postman_collection.json -e ServeRestEnvi.postman_environment.json -r cli
```
- Run tests with report
```
newman run ServeRest.postman_collection.json -e ServeRestEnvi.postman_environment.json -r cli,htmlextra
```
### Report 

If you chose to run the tests with the htmlextra report, you generated an html file with the results of the tests and to check the validations you can open the **newman** folder that was created in the location where the collection and environment files are located.

## Contact

vagnerosales@gmail.com


