


# Hosting a Full-Stack Application

# Udagram

This application is  The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application. It has been deployed via pipeline and hosted [here](https://779300618230-aws-bucket.s3.us-east-2.amazonaws.com/index.html)


### General Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```
### Front End App Dependencies

  * angular/common
  * angular/core
  * angular/forms
  * angular/http
  * angular/platform-browser
  * angular/platform-browser-dynamic
  * angular/router
  * ionic-native/core
  * ionic-native/splash-screen
  * ionic-native/status-bar
  * ionic/angular
  * core-js
  * rxjs
  * typescript

### Back End API Dependencies

  * bcryptjs
  * jsonwebtoken
  * aws-sdk
  * body-parser
  * cors
  * dotenv
  * email-validator
  * express
  * pg
  * reflect-metadata
  * sequelize
  * sequelize-typescript

### Hosting Infrastructure

The Front end is hosted on an AWS S3 Bucket and the back end an Elsatic Beanstalk instance, behind this there is a postgresql database also hosted on AWS RDS. 
![image](https://github.com/daniel-tickell/nd0067-c4-deployment-process-project-starter/blob/master/docs/Service%20Diagram.jpg)

### Deployment Pipeline 

The Deployment pipeline uses Circleci to sync changes to this repo, by building and deploying to AWS
The deployment process looks like this
![image](https://github.com/daniel-tickell/nd0067-c4-deployment-process-project-starter/blob/master/docs/Pipeline%20overview.jpg)

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework
