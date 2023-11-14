# Whril API - Serverless API Gateway

![Project Cover](/images/whril_api.jpg)

Whril API is a serverless API gateway built using Node.js and Express, utilizing Axios for seamless HTTP requests. It is designed to be deployed on Google Cloud Functions and utilizes the Functions Framework for easy deployment and scaling.

## Features

- **Inbuilt Authentication:** Secure your APIs with a built-in authentication system. Easily manage and authenticate users within the gateway.

- **Proxy Routing:** Route requests to different microservices or external APIs based on configurable rules.

- **Rate Limiting:** Protect your APIs from abuse by implementing rate limiting. Control the number of requests a client can make within a specified time frame.

- **Logging:** Comprehensive logging of requests and responses for debugging and auditing purposes.

- **Monitoring:** Monitor the health and performance of your API Gateway with built-in tools.

- **Google Cloud Functions:** Deploy Whril API effortlessly on Google Cloud Functions, taking advantage of the serverless infrastructure.

- **Functions Framework:** Use the Functions Framework to simplify the deployment process and focus on writing code.

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js

- Firebase service account keys: Place your Firebase service account keys in the `secrets/firebase.json` file.

## Getting Started

1. Clone the repository:

   ```bash
    git clone https://github.com/its-saran/whril-api.git

2. Navigate to the project directory:

    ```bash
    cd whril-api

3. Install dependencies:

    ```bash
    npm install

3. Configure API Gateway:

    - Customize the endpoints, rate limiting settings, and other configurations in config/config.json.

    - Example endpoints are shown in config.json

4. Run the Whril API locally:

    ```bash=
    npm start
    ```

    The API will be accessible at http://localhost:3000.

## Deployment

1. To deploy

    ```bash=
    npm run deploy
    ```

2. You can configure the deployment settings, such as timeout, memory, max instances, etc., of the cloud functions in package.json.