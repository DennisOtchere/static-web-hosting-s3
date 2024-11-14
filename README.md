# Static Website Hosting on Amazon S3

### Project Overview
This project demonstrates how to host a static website using Amazon S3 (Simple Storage Service). In about 30 minutes, we set up an S3 bucket, uploaded website files, enabled static website hosting, and managed permissions to make the site publicly accessible. This guide covers each step in detail, with additional insights and troubleshooting tips.

> **Project Time**: 30 minutes  
> **Project Guide**: ([NextWork](https://community.nextwork.org/c/all-aws-projects/))

### Table of Contents
1. [About Amazon S3](#about-amazon-s3)
2. [Project Setup](#project-setup)
   - [Create an S3 Bucket](#create-an-s3-bucket)
   - [Upload Website Files](#upload-website-files)
   - [Enable Static Website Hosting](#enable-static-website-hosting)
   - [Adjust Permissions](#adjust-permissions)
3. [Troubleshooting](#troubleshooting)
4. [Additional Resources](#additional-resources)

---

## About Amazon S3
Amazon S3 is a scalable cloud storage service by AWS, ideal for hosting static websites due to its high durability, availability, and ease of use. Hosting a website on S3 allows you to make your content publicly accessible and deliver it with high availability.

## Project Setup

### 1. Create an S3 Bucket
   - Go to the [AWS S3 Console](https://aws.amazon.com/s3/).
   - Create a new bucket with a globally unique name.
   - For this project, we used the **US East (N. Virginia)** region (`us-east-1`), but you can select a region that best suits your needs.

### 2. Upload Website Files
   - Upload your `index.html` and other necessary assets (e.g., images or stylesheets) to the S3 bucket.
   - Ensure all assets are correctly referenced in the `index.html` file for smooth loading.

### 3. Enable Static Website Hosting
   - Go to the **Properties** tab of your S3 bucket.
   - Under **Static website hosting**, select **Enable** and specify the `index.html` as the default document.
   - Save your changes.

### 4. Adjust Permissions
   - To make the website publicly accessible, navigate to the **Permissions** tab.
   - Disable the "Block all public access" setting if necessary.
   - Update the bucket's Access Control List (ACL) to allow public access to the contents.

## Troubleshooting
   - If you see a "403 Forbidden" error when accessing the bucket's endpoint URL, check the following:
      - Ensure public access is enabled.
      - Verify that permissions are correctly set for the bucket and its objects.
      - Confirm that your `index.html` file is properly named and accessible.

## Additional Resources
For a detailed step-by-step guide with screenshots, refer to the PDF document included in this repository: [Hosting a Website on Amazon S3](legendary-aws-host-a-website-on-s3.pdf).

---

### Credits
This project was completed with the support of the NextWork community, a fantastic resource for hands-on learning in cloud and tech skills. Visit [NextWork](https://community.nextwork.org) for more information.
