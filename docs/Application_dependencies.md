# Application Dependencies

This document outlines the dependencies for the Angular project, including client-side libraries, server-side technologies, and AWS services used for hosting and deployment.

## Project Overview
- **Frontend Framework:** Angular
- **Hosting Platform:** AWS (S3, Elastic Beanstalk, RDS)
- **Purpose:** [This application is the social media platform Udagram, which allows users to create an account and post images with brief descriptions to the application.]


## Frontend Dependencies

### Angular Framework
- Version: 8.2.14

### Node.js and npm
- Node.js: v18.20.5
- npm: v10.8.2


## Backend/Server Dependencies

### Runtime
- Node.js: v18.20.5 (used in Elastic Beanstalk for the API/backend)

### Database
- **AWS RDS:** PostgreSQL 13.18


## Hosting and Deployment

### AWS Services
1. **S3**: For hosting the static files
   - Bucket Name: `mybucket193871254100`
   - Region: us-east-1

2. **Elastic Beanstalk**: For deploying the backend
   - Environment Name: `udagram-api-dev `
   - Instance Type: t2.medium
   - Platform: Node.js

3. **RDS**: For database storage.
   - Database Engine: PostgreSQL
   - Version: 13.18
   - Instance Type: db.t3.micro
   - Security Group: `awseb-e-ib2n8v8z9j-stack-AWSEBSecurityGroup-JH5mlegngK8W`
