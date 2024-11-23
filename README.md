# My Portfolio Website Hosting on Amazon S3

### Project Overview
This project demonstrates how to host a  website using Amazon S3 (Simple Storage Service). The project involves setting up an S3 bucket, uploading website files, enabling static website hosting, and managed permissions to make the site publicly accessible. This guide covers each step in detail, with additional insights and troubleshooting tips.



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

## Resources
The files for the website can be found in the portfolio folder in this same repository


> The hosted website can be viewed at
[Click Here](https://anabi-asah-portfolio.s3.us-east-1.amazonaws.com/index.html)

---

### Contact
For further assistance on project set up, you can reach out to me through [email](anabiasah@gmail.com)

