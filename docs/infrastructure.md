## Udagram Infrastructure

Main project arhitecture will be found [here](https://github.com/khaledomar77/Hosting-full-stack-application/blob/main/docs/Main_architecture.jpg)

## AWS
### RDS Postgres

The application server uses AWS RDS Postgres as database for storing and retrieving information.

Database URI: postgresql://postgres:password@postgres.database-1.c5ewrpjs7njq.us-east-1.rds.amazonaws.com

Elastic Beanstalk

The application server is deployed on AWS Elastic Beanstalk service. The application is build, archived and uploaded to and S3 bucket from where Elastic Beanstalk extracts and runs the application on an endpoint.

EB URL: http://udagram-api-dev.eba-43ppftpt.us-east-1.elasticbeanstalk.com/

### S3 Bucket

The frontend application is deployed using AWS S3 Bucket. The bundled assets are uploaded to an S3 bucket and that bucket is made publicly readable.

Bucket URL: http://khaled-udagram.s3-website-us-east-1.amazonaws.com/home

End users can access the application from the Bucket URL.
