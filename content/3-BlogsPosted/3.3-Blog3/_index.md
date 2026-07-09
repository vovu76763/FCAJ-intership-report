---
title: "Blog 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---
# INTEGRATING IAM COMPUTE ROLES FOR SERVER-SIDE RENDERING APPS ON AWS AMPLIFY HOSTING

When building Server-Side Rendering applications such as Next.js or Nuxt on AWS, one common challenge is how the application can securely access AWS services without storing Access Keys or Secret Keys in source code or environment variables.

To address this need, AWS Amplify Hosting introduced the IAM Compute Roles feature for SSR applications.

![IAM Compute Roles flow for SSR applications on AWS Amplify Hosting](/images/3-BlogsPosted/3.3-Blog3/blog-3.jpg)

## 1. What are IAM Compute Roles?

IAM Compute Roles allow an IAM Role to be attached directly to the runtime environment of an SSR application on Amplify Hosting.

As a result, server-side code can access AWS services through a temporary-credential mechanism similar to an EC2 Instance Profile or a Lambda Execution Role.

## 2. Common use cases

* Accessing AWS Secrets Manager or Systems Manager Parameter Store to retrieve configuration values.
* Connecting to Amazon RDS or Amazon DynamoDB without storing credentials in the application.
* Calling AWS service APIs from the server side.
* Setting different access permissions across development, staging, and production environments.

## 3. Implementation example

In AWS's tutorial, a Next.js application is configured to access a private Amazon S3 bucket.

The process includes:

1. Create an IAM Role with read permissions for S3.
2. Grant Amplify Hosting permission to use this role.
3. Deploy the Next.js application to Amplify.
4. Use the AWS SDK inside an API Route to access the data from S3.

Thanks to IAM Compute Roles, the application can authenticate with AWS without storing Access Keys or Secret Keys in the source code.

## 4. Conclusion

IAM Compute Roles simplify AWS access management for SSR applications on Amplify Hosting. This is a useful feature for systems that need server-side access to AWS resources while still upholding security and access-governance principles.

📖 **Original article:** [aws.amazon.com/blogs/mobile/iam-compute-roles-for-server-side-rendering-with-aws-amplify-hosting](https://aws.amazon.com/blogs/mobile/iam-compute-roles-for-server-side-rendering-with-aws-amplify-hosting/)

🔗 **Link to the post in the FCJ group:** [facebook.com/share/p/1PEvrCKJsS](https://www.facebook.com/share/p/1PEvrCKJsS/)
