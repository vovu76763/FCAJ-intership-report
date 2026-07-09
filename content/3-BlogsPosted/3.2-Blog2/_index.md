---
title: "Blog 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---
# EMBEDDING A GENAI ASSISTANT INTO AN INTERNAL APPLICATION WITH AWS AMPLIFY, CDK AND AMAZON Q BUSINESS

As the volume of internal documentation keeps growing, traditional keyword-based search often fails to meet users' needs. Instead of searching through documents one by one, many organizations are moving toward AI assistants capable of answering natural-language questions based on enterprise data.

A recent AWS blog post walks through how to build this model using Amazon Q Business combined with AWS Amplify and AWS CDK.

![Architecture for embedding a GenAI assistant with AWS Amplify, CDK and Amazon Q Business](/images/3-BlogsPosted/3.2-Blog2/blog-2.jpg)

## 1. Solution overview

The architecture uses:

* Amazon Q Business to provide question-answering capabilities based on internal data.
* AWS Amplify Gen 2 to build and deploy the application.
* AWS CDK to manage infrastructure as code.
* Amazon Cognito and IAM Identity Center for authentication and authorization.
* Amazon S3 to store documents for the data-indexing process.

## 2. How the architecture works

1. The user signs in to the application through Cognito.
2. Internal documents are uploaded to Amazon S3.
3. Amazon Q Business is granted access and indexes the data from S3.
4. A chat interface is embedded directly into the web application.
5. Users can ask questions and receive answers based on enterprise data, along with reference sources.

## 3. Notable highlights

One thing I found quite useful is that most of the infrastructure and access configuration is implemented using AWS CDK. This significantly reduces manual configuration work and makes it easier to manage environments through Infrastructure as Code.

In addition, using Amazon Q Business helps organizations roll out GenAI features faster without having to build or operate their own AI models.

## 4. Conclusion

Integrating AI assistants into internal applications is becoming a common need across many organizations. The architecture using Amazon Q Business, Amplify, and CDK is a worthwhile approach for systems that need to surface knowledge from enterprise documents in a secure and controlled way.

📖 **Original article:** [aws.amazon.com/blogs/mobile/from-build-to-embed-creating-and-embedding-genai-apps-with-aws-amplify-cdk-and-amazon-q-business](https://aws.amazon.com/blogs/mobile/from-build-to-embed-creating-and-embedding-genai-apps-with-aws-amplify-cdk-and-amazon-q-business/)

🔗 **Link to the post in the FCJ group:** [facebook.com/share/p/1BkgmtmwUw](https://www.facebook.com/share/p/1BkgmtmwUw/)
