# simple-terraform-project
Simple DevOps project to Practice Terraform with AWS and create a Static website on S3


S3 Static Website Project with Terraform
This project demonstrates how to create an S3 bucket on AWS and set up static website hosting using Terraform. It's a great way to showcase your portfolio projects or CV on AWS.
Project Goal
The main aim was to automate the creation of an S3 bucket and configure it to serve a static website using Terraform. This includes setting up the necessary configurations, uploading website files, and making the bucket publicly accessible, all through code.
Steps Implemented
Here’s how I approached the project:
•
Created an S3 bucket using Terraform.
•
Enabled the settings required to set up static website hosting on the S3 bucket.
•
Uploaded website files like index.html, error.html, and images to the S3 bucket using Terraform.
•
Enabled public access to the bucket via Terraform.
•
Optionally, you can connect the S3 website with a domain name, or just use the S3 endpoint.
•
Tested the website by pasting the website endpoint in a browser.
Key Files
These are the key files in the project:
•
providers.tf: This file contains the provider details for AWS, specifying the AWS provider and the region.
•
main.tf: This file contains the core logic to create the S3 bucket and configure it for static website hosting.
•
variables.tf: This file defines the variables used in the project, such as the bucket name.
•
outputs.tf: This file defines the outputs, such as the website endpoint.
Terraform Commands Used
Here are some of the key Terraform commands I used:
•
terraform init: Initialises Terraform and downloads the required dependencies.
•
terraform plan: Shows what Terraform is going to do based on the configuration.
•
terraform apply -auto-approve: Creates the resources without asking for confirmation.
Making the Bucket Public
To make the bucket public, I did the following:
•
Refined the bucket ownership.
•
Used a public access block resource.
•
Used S3 bucket ACL (Access Control List).
Uploading Objects
I uploaded objects (like HTML and image files) using the resource "aws_s3_object". Key configurations included specifying the bucket, key, and source for each object.
Website Configuration
To configure the website, I used the AWS S3 website configuration resource. This required specifying an index document and an error document.
Tools Used
•
Terraform: For Infrastructure as Code.
•
AWS: As the cloud provider.
•
Visual Studio Code (VS Code): For editing the code.
•
I hope this helps you understand the project and how it was implemented!
