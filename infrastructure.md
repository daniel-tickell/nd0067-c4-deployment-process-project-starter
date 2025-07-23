# Hosting Infrastructure

The Front end is hosted on an AWS S3 Bucket and the back end an Elsatic Beanstalk instance, behind this there is a postgresql database also hosted on AWS RDS. 
![image](https://github.com/daniel-tickell/nd0067-c4-deployment-process-project-starter/blob/master/docs/Service%20Diagram.jpg)

## S3 Bucket
The bucket 779300618230-aws-bucket is used to host the front end application static files, these are uploaded and deployed as part of the circleci process.

## Elastic Beanstalk
The elsastic beanstalk instance (udagram-api-dev) is used to host the back end api, the application is deployed as a zip file as part of the circleci deployment and built on the server.
Environment variables are configured here and are deployed to AWS as part of the [deploy.sh](https://github.com/daniel-tickell/nd0067-c4-deployment-process-project-starter/blob/master/udagram/udagram-frontend/bin/deploy.sh) script

## RDS
RDS is a hosted postgresql instance on AWS that is used for the back end to create and store data related to the site operations. 

## Circleci
Circleci is used to monitor the github repo for changes and kick off a build and deploy task when changes are detected. See [Pipeline](https://github.com/daniel-tickell/nd0067-c4-deployment-process-project-starter/blob/master/pipeline.md) for more information.

## Github
Github is used to host the source code for the application and provide version control for changes. 
