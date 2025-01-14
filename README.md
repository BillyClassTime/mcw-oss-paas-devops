# OSS PaaS and DevOps workshop

This repository contains resources for use with the OSS PaaS and DevOps workshop, including the starter MERN app, code for Azure Functions, scripts for seeding data into the MongoDB database, as well as exporting data, and an ARM template for deploying the Lab virtual machine (VM) to Azure.

## LabVM

To get started, click the Deploy to Azure link below. This will provision a fully configured Linux Lab VM, used as a development machine for the OSS PaaS and DevOps workshop. This should be completed before your workshop.

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fzoinertejada%2Fmcw-oss-paas-devops%2Fmaster%2FLabVM%2Fazure-deploy.json)

VM details:

1. Ubuntu Server 16.04 LTS
2. Docker Community Edition
3. Visual Studio Code
4. Node.js and NPM
5. Mongo DB Community Edition
6. Opens port 3389 to allow RDP connections

## Starter app

Once the VM is deployed, connect to it using an RDP client, fork the starter application into your own GitHub repo, and clone it to the Lab VM.

The starter project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).

In the project directory, run:

```sh
npm install
node data/Seed.js
npm run build
npm start
```

### `npm install`

Installs required components.

### `node data/Seed.js`

Seeds the local MondoDB database with sample data.

### `npm run build`

Builds the app for production to the `build` folder. It correctly bundles React in production mode and optimizes the build for the best performance. The build is minified and the filenames include the hashes.

Your app is ready to be deployed!

### `npm start`

Runs the app in the development mode. You will also see any lint errors in the console.

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

mongodb://best-for-you-db-40533-g:43JNjT9StUlseaEXbtBQ4R8u9EFzbu5vX4WO018jvlHb2cbtlV8HQw9jTcpN8kL7cVdeXMGVr15y2hAJtiG0pg==@best-for-you-db-40533-g.documents.azure.com:10255/?ssl=true&replicaSet=globaldb

mongoimport --host best-for-you-db-40533-g.documents.azure.com:10255 -u best-for-you-db-40533-g -p 43JNjT9StUlseaEXbtBQ4R8u9EFzbu5vX4WO018jvlHb2cbtlV8HQw9jTcpN8kL7cVdeXMGVr15y2hAJtiG0pg== --db
best-for-you-organics --collection plans --ssl --sslAllowInvalidCertificates --type
json --file ~/MongoExport/plans.json


bestforyouregistry40553g.azurecr.io/best-for-you-organics:latest


bestforyouregistry40553g.azurecr.io
bestforyouregistry40553G
tFYogvU5kuvxob1X2uO+XeWXIsv3ua6A

Ghl8TJQ8YjSZ442xtx

sv2xxsnh6nad2bpjmlj7lvnzjw6hujgxhme6w6itd5asmyw4abtq

Password.1!!
