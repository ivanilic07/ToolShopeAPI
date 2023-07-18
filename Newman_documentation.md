# Running Tests in Command Line with Newman

Newman is a command-line collection runner for Postman that allows you to run and test a Postman collection directly from the command line. 

## **Prerequisites**
Ensure that you have the following installed:
1. Node.js (Version 10 or higher)
2. npm (Comes with Node.js)
3. Postman (To create and export the collection)

## **Installation of Newman**
After you've installed Node.js and npm, you can install Newman globally on your system. Run the following command in your command line:
npm install -g newman



## **Running Newman**
To run Newman, you'll need a Postman Collection. Follow the steps below:

1. **Export your Postman Collection**
   - Open Postman
   - Find your collection
   - Click on the three dots next to the collection name
   - Click "Export"
   - Save the file in a location that you can easily access

2. **Run the Collection with Newman**
   - Use the `run` command followed by the location of the collection

newman run Dhimahi.postman_collection.json


If your collection file is in another directory, provide the full path:
newman run /path/to/your/collection/Dhimahi.postman_collection.json


## **Further Options**

Newman provides numerous options for the `run` command that lets you customize the run, including specifying an environment, setting global variables, defining iteration data, etc.

- **Specify an Environment**
  - Export your environment from Postman
  - Run your collection with the `-e` or `--environment` option

newman run mycollection.postman_collection.json -e Dhimahi.postman_environment.json


For a full list of options and usage details, check the [official Newman documentation](https://learning.postman.com/docs/running-collections/using-newman-cli/command-line-integration-with-newman/).






