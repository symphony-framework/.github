# Symphony

## About Symphony

Welcome to Symphony, a framework that helps developers deploy real-time collaborative applications easily. In this document, we will guide you through the steps to get started with Symphony.

## Getting Started

### Prerequisites

To use Symphony, you must have the following prerequisites installed on your system:

- Amazon Web Services CLI
- Node.js

You can download and install these tools from their respective official websites. Once you have installed these tools, follow the steps below to configure the AWS CLI tool with your access token.

Configuring AWS CLI tool:
1. Open your command-line interface (CLI) and enter the following command: `aws configure`.
2. Enter your AWS access key ID and secret access key when prompted.
3. Choose a default region and output format.
4. Press Enter to confirm your inputs.

For further details, please see the [official docs](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-quickstart.html).

Once you have installed the dependencies and configured the AWS CLI tool, you can proceed with the installation of the Symphony CLI tool.

### Installing the CLI

Before starting a Symphony project, you’ll need to download the Symphony CLI tool from npm.

Run `npm install -g symphony-cli` to install the CLI globally.

Once the installation is complete, you can get started with your first real-time collaborative application powered by Symphony.

### Creating a Symphony Application

1. Create a new directory and initialize a new node project by running `npm init`.
1. Install the Symphony client by running `npm i @symphony-rtc/client`.
1. Create a `symphony.config.js` file. Within this file, create a new instance of the Symphony client: `import { SymphonyClient } from "@symphony-rtc/client";`. Pass in your domain name for the project as an argument. When you’re done, export the client for use in your project i.e. `export default client`.
1. Write your application code using the conflict-free data types provided by Symphony.
1. When you’re done, run the command `symphony-cli compose` to deploy your application on AWS.

Once all your infrastructure has been provisioned, you’re ready to go. You’ve just deployed a real-time collaborative application in 5 steps. You can open your developer dashboard on localhost by running `symphony-cli dashboard`.
