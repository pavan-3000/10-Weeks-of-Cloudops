# Static Website Hosting on AWS with CI/CD (Using AWS Management Console)

## Introduction
This project involves hosting a static website on AWS using the Management Console. I utilized Amazon S3 for storage, CloudFront for content delivery, while implementing a CI/CD pipeline for automated deployments.

## Technologies Used
- **Amazon S3**: For storing static website files.
- **CloudFront**: To improve content delivery speed.
- **CI/CD Tools**: AWS CodePipeline.

## Architecture Diagram
![Architecture Diagram](link-to-your-diagram)

## Step-by-Step Guide
### 1. Setting Up the S3 Bucket
- Go to the AWS Management Console.
- Navigate to **S3** and click on **Create bucket**.
- Enter a unique bucket name and select your desired region.
- Enable **Block all public access** settings, and create the bucket.
- Upload your static website files to the bucket.

![S3 Bucket Setup Screenshot](link-to-screenshot)

### 2. Configuring Bucket Policy
- After uploading, go to the **Permissions** tab of your bucket.
- Click on **Bucket Policy** and add a policy to allow public read access.


