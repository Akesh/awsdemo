# Build and Deployment automation using AWS Elastic Beanstalk and Jenkins 
This is a maven application and is used to automate build and deployment process using below components 
a. Amazon Elastic Beanstalk - as an application environment running Docker container
b. Amazon S3 Services - Storage of revisions/builds 
c. Jenkins - as a build tool

Whenever push event happens in GIT,jenkins will read this event and start building our application.
After successfull build Jenkins will push build to S3 and start deploying application to docker container via elastic beanstalk.
