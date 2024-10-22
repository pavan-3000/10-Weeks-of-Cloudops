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

### 2. Setting Up CloudFront
- Navigate to **CloudFront** in the AWS Management Console.
- Click on **Create Distribution** and select **Web**.
- For **Origin Domain Name**, choose your S3 bucket.
- Configure the remaining settings as needed, including enabling caching and setting TTL (Time to Live) values.
- Click on **Create Distribution** to complete the setup.

### 3. Configuring Route 53
- Go to **Route 53** in the AWS Management Console.
- Create a **Hosted Zone** for your domain if you haven't already.
- Set up **A records** pointing to your CloudFront distribution:
  - Select **Alias** as **Yes**.
  - Choose your CloudFront distribution from the list.

### 4. Implementing CI/CD with AWS CodePipeline
- Navigate to **CodePipeline** and click on **Create pipeline**.
- Configure the pipeline settings:
  - Choose a **source provider** (e.g., GitHub) and authenticate it.
  - Set up the **build stage** (if applicable), using AWS CodeBuild or another service.
  - For the **deploy stage**, select your S3 bucket to automate deployment on code changes.
- Save and create the pipeline to enable automatic deployments.



