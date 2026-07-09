---
title: "Blog 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# BUILDING AN OFFLINE-FIRST APPLICATION WITH AWS AMPLIFY, TANSTACK QUERY, APPSYNC AND MONGODB ATLAS

When using web or mobile applications under unstable network conditions, users often experience slow data loading, interrupted operations, or even data loss when offline. To deliver a smoother experience, many systems today adopt the Offline-First model combined with Optimistic UI.

A recent AWS blog post introduces how to build this architecture by combining AWS Amplify, AWS AppSync, TanStack Query, and MongoDB Atlas.

![Offline-First architecture with AWS Amplify, TanStack Query, AppSync and MongoDB Atlas](/images/3-BlogsPosted/3.1-Blog1/blog-1.png)

## 1. Solution overview

The architecture uses:

* AWS Amplify Gen 2 to build and deploy the full-stack application.
* AWS AppSync to provide a GraphQL API for data synchronization.
* TanStack Query to manage client-side data, supporting caching and optimistic updates.
* MongoDB Atlas as the backend database.

In addition, the system uses AWS Lambda for serverless processing and Amazon Cognito for user authentication.

## 2. How does Optimistic UI work?

Instead of waiting for a response from the server before updating the interface, Optimistic UI allows the application to display the expected result immediately after the user performs an action.

For example, when creating a new task in a To-do app:

* The interface immediately displays the new task.
* A request is sent to AppSync to persist the data.
* If the request succeeds, the data is synchronized as normal.
* If an error occurs or the connection is lost, the previous state is restored through a rollback mechanism.

This approach makes the application feel more responsive and reduces the perceived waiting time for users.

## 3. Processing flow

1. The user performs a data-creation action.
2. TanStack Query updates the local cache and immediately displays the result on the UI.
3. The request is sent to AppSync via GraphQL.
4. AppSync processes the request and stores the data in MongoDB Atlas.
5. If an error occurs, the cached data is rolled back to its previous state.

In AWS's example, conflict resolution is implemented on a First-Come, First-Served basis.

## 4. Conclusion

Offline-First and Optimistic UI are becoming important techniques for improving user experience in modern applications. With Amplify, AppSync, and TanStack Query, implementing these features becomes simpler while still ensuring data synchronization once network connectivity is restored.

📖 **Original article:** [aws.amazon.com/blogs/mobile/offline-caching-with-aws-amplify-tanstack-appsync-and-mongodb-atlas](https://aws.amazon.com/blogs/mobile/offline-caching-with-aws-amplify-tanstack-appsync-and-mongodb-atlas/)

🔗 **Link to the post in the FCJ group:** [facebook.com/groups/awsstudygroupfcj/permalink/2190116435086650](https://www.facebook.com/groups/awsstudygroupfcj/permalink/2190116435086650/)
