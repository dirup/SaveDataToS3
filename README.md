# SaveDataToS3
This service is responsible for connecting to S3 and push the data(which was pulled from Salesforce) from local file system to S3 . 

This Microservice is developed using Springboot. Current project structure is the general template structure using Springboot.

The main component in this microservice is BucketController,AmazonClient. AmazonClient is used to connect to S3 bucket using the credentials saved in application.properties file.
and BucketController is the component used to save the data to S3.

All the configurable properties in this microservices like username, password, bucketname, accesskey, secretkey are maintained in application.properties under resources folder
file, so it is easy to configure them even in runtime and supports loose coupling.

Amazon aws sdk for java is required to connect to Amazon AWS S3 bucket using java code.
