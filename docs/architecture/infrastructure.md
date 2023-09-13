## Udagram Infrastructure

![Architecture](architecture.png)

### AWS
#### RDS Postgres
- RDS - Database Host: postgres.cngwc09xasdk.us-east-1.rds.amazonaws.com
- RDS - Database Port: 5432
- RDS - Database Name: postgres

#### Elastic Beanstalk
The application server is deployed on AWS Elastic Beanstalk service. The application is build, archived and uploaded
to and S3 bucket from where Elastic Beanstalk extracts and runs the application on an endpoint.

EB URL: `http://udagram-api-last.eba-ipgvrked.us-east-1.elasticbeanstalk.com/`

#### S3 Bucket
The frontend application is deployed using AWS S3 Bucket. The bundled assets are uploaded to an S3 bucket and that
bucket is made publicly readable.

Bucket URL: `http://udagram-frontend-last.s3-website-us-east-1.amazonaws.com/`

End users can access the application from the Bucket URL.
