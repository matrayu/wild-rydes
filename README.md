![Wild-Rydes Homepage](https://webapp.serverlessworkshops.io/images/wildrydes-homepage.png)

# Wild Rydes README

Welcome to Wild Rydes! This demo application showcases the innovative use of AWS services to build a serverless web application that simulates a ride-sharing service, allowing users to request rides from "unicorns" and get to their destinations faster and hassle-free.

To see this app in action, please visit [Wild Rydes](https://main.d21rvi7airpu6a.amplifyapp.com/) and sign up.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Architecture](#architecture)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [User Management](#user-management)
- [Backend Processing](#backend-processing)
- [RESTful API](#restful-api)
- [Deployment](#deployment)
- [Security](#security)
- [Contributing](#contributing)

## Introduction

Wild Rydes is a conceptual ride-sharing application developed by the team at AWS. The application presents users with an HTML-based user interface for indicating their pickup location and interfaces on the backend with a RESTful web service to submit ride requests and dispatch a nearby unicorn.

## Features

- **User Registration and Authentication:** Users can register and authenticate using Amazon Cognito, ensuring secure access to the application.
- **Ride Requests:** Users can request rides through a simple web interface, specifying their location and destination.
- **Serverless Backend:** Utilizes AWS Lambda and Amazon API Gateway for handling ride requests without the need for managing server infrastructure.
- **Data Storage:** User data and ride information are stored in Amazon DynamoDB, providing fast and scalable storage solutions.
- **Static Web Hosting:** The web interface is hosted using AWS Amplify Console, serving static resources from Amazon S3 and delivering content through Amazon CloudFront.

## Architecture

Wild Rydes leverages a serverless architecture, simplifying operations and reducing the need to manage infrastructure. The architecture includes:

- **Amazon S3 and AWS Amplify Console** for hosting static web resources.
- **Amazon Cognito** for user registration, authentication, and management.
- **AWS Lambda** for executing backend logic in response to web application events.
- **Amazon API Gateway** for creating a RESTful API that interfaces between the frontend and backend.
- **Amazon DynamoDB** for storing and retrieving ride and user data efficiently.

![Architecture-Diagram](https://webapp.serverlessworkshops.io/images/wildrydes-complete-architecture.png)

## Technology Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** AWS Lambda (Node.js)
- **Database:** Amazon DynamoDB
- **Authentication:** Amazon Cognito
- **API:** Amazon API Gateway
- **Hosting:** AWS Amplify Console, Amazon S3

## Getting Started

To replicate this project in your AWS account, follow the instructions provided by AWS:

[WELCOME TO WILD RYDES WORKSHOP!](https://webapp.serverlessworkshops.io/)

## User Management

Users must register and confirm their accounts through Amazon Cognito. The registration process requires only an email address and password. Amazon Cognito sends a confirmation email with a verification code to complete the registration.

![Authentication Architecture](https://webapp.serverlessworkshops.io/images/restful-api-architecture.png)

## Backend Processing

The backend processing is handled by AWS Lambda functions, which are triggered by API requests to dispatch unicorns and record the ride details in Amazon DynamoDB.

![Serverless Backend Architecture](https://webapp.serverlessworkshops.io/images/serverless-backend-architecture.png)

## RESTful API

The RESTful API built with Amazon API Gateway exposes endpoints for registering users, requesting rides, and querying the status of the ride. It's secured with Amazon Cognito user pools, ensuring that only authenticated users can access the API.

![Restful API Architecture](https://webapp.serverlessworkshops.io/images/restful-api-architecture.png)

## Deployment

The entire application is deployable with minimal manual intervention using AWS Amplify Console, which automatically provisions and configures the necessary AWS services.

![Amplify Deployment](https://webapp.serverlessworkshops.io/images/amplify-deploy-status.png)

## Security

Wild Rydes uses AWS best practices for security, including HTTPS for all communication, token-based authentication with Amazon Cognito, and fine-grained access control with AWS IAM.

## Rebuild

For more detailed documentation on each component of Wild Rydes, refer to the AWS documentation provided in the [Getting Started](#getting-started) section.

This README is designed to provide a comprehensive overview of the Wild Rydes application, demonstrating the power and simplicity of building serverless applications with AWS.
