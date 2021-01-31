# Serverless AWS-NodeJs intial setup :hammer:

Of all the things I am a fan of, Serverless is one of them. Needless to say that, serverless in the future and the present. Working with it is super fun and interesting, so I thought of building something that can quickly get you started with it. 

# What does it do? 🤔

Serverless is a vast topic and working with it requires you to write a lot of things from scratch. I made it easier for you, by automating the initial setup. 
You will get pre-made user functions for CRUD operation with cognito authorizer, Webpack configs, basic cognito setup, one dummy s3 bucket and function to upoad images on s3 and db clients for s3 and dynamodb with status codes.




# More details on what this project offers you 👇 
- **User create, update, get, deltete, deactivate functions in DynamoDB table and to delete cognito user**
- **Cognito authorizer**
- **One Demo S3 bucket**
- **Lambda to upload images to S3**
- **DB and S3 clients**
- **Cognito client**
- **Status codes**
- **Code formatter**
- **Webpack configs**
- **development and production stages**
---

# How do you use it?

All you need to do this, fork this repo and follow the steps mentioned below. 

# Requirements

- [Install the Serverless Framework](https://serverless.com/framework/docs/providers/aws/guide/installation/)
- [Configure your AWS CLI](https://serverless.com/framework/docs/providers/aws/guide/credentials/)

# Installation

To create a new Serverless project.

``` bash
$ serverless install --url https://github.com/GM1957/serverless-aws-nodejs-initial-setup
```

Enter the new directory

``` bash
$ cd serverless-aws-nodejs-initial-setup
```

Install the Node.js packages

``` bash
$ npm install
```

### Usage

To run a function on your local

``` bash
$ serverless invoke local -f Users -p ./pathToYour_input.json --stage dev
```

To simulate API Gateway locally using [serverless-offline](https://github.com/dherault/serverless-offline)

``` bash
$ serverless offline --stage dev
```

Deploy your project in development stage

``` bash
$ serverless deploy --stage dev
```
Deploy your project in production stage

``` bash
$ serverless deploy --stage prod
```

Deploy a single function in development

``` bash
$ serverless deploy FunctionName --stage dev
```

# Running code formatCheck

Run your check using [now there is only the code format checker test]

``` bash
$ npm run formatCheck
```
# Running code formatter

format all the codes with pritter formatter

``` bash
$ npm run format
```
