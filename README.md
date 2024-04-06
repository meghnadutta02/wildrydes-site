# Application Overview

This application leverages various AWS services to create a serverless architecture for hosting and managing web resources, user authentication, and data storage. It utilizes AWS Lambda, Amazon API Gateway, Amazon DynamoDB, Amazon Cognito, and AWS Amplify Console.

## Components

### AWS Lambda

AWS Lambda is used for running serverless functions in response to events such as HTTP requests. In this application, Lambda functions handle backend API logic and interact with other AWS services like DynamoDB.

### Amazon API Gateway

Amazon API Gateway provides a fully managed service for creating, deploying, and managing APIs at scale. In this architecture, API Gateway acts as the frontend to the backend Lambda functions, exposing endpoints for clients to interact with.

### Amazon DynamoDB

Amazon DynamoDB is a fully managed NoSQL database service provided by AWS. In this application, DynamoDB serves as the persistence layer for storing data managed by the backend Lambda functions.

### Amazon Cognito

Amazon Cognito provides user authentication and management functions for securing the backend API. It allows users to sign in through various identity providers and provides features like multi-factor authentication and user pool management.

### AWS Amplify Console

AWS Amplify Console offers continuous deployment and hosting for static web resources, including HTML, CSS, JavaScript, and image files. It simplifies the process of deploying and managing frontend assets while providing features like custom domains and HTTPS support.

## Architecture

The architecture of the application is as follows:

1. **Frontend Hosting**: Static web resources such as HTML, CSS, and JavaScript files are hosted and deployed using AWS Amplify Console.

2. **User Authentication**: Amazon Cognito handles user authentication, allowing users to sign in securely and obtain access tokens for interacting with the backend API.

3. **Backend API**: AWS Lambda functions integrated with Amazon API Gateway serve as the backend for the application, executing logic and interacting with DynamoDB to store and retrieve data.

4. **Data Storage**: Amazon DynamoDB provides a scalable and highly available NoSQL database for persisting data managed by the backend API.

![Architecture Image](Serverless_Architecture.d930970c77b382db6e0395198aacccd8a27fefb7.png)


## License

This project is licensed under the [MIT License](LICENSE).
