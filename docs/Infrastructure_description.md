# Infrastructure description

The application utilizes various AWS components to host the API, Front-End, and Database. First, the API is hosted using Elastic Beanstalk, which serves as the application server. Second, the Front-End is hosted on an S3 bucket as a static website, where all the necessary files for the Front-End are stored. Finally, the managed relational Database is a PostgreSQL instance hosted on RDS.


## How everything works together

1. The end user goes on a site and is thereby calling the client (S3 Bucket).
2. The S3 Bucket is fetching data from the Udagram API on Elastic Beanstalk.
3. Elastic Beanstalk saves data on the RDS Postgres DB.