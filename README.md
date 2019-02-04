# Blockchain: Connect Private Blockchain to Front-End Client via APIs

[![Build Status](https://semaphoreci.com/api/v1/vdagar/blockchain_frontend/branches/master/badge.svg)](https://semaphoreci.com/vdagar/blockchain_frontend)

In Project 2: Create Your Own Private Blockchain, you solved the challenge of how to persist our blockchain dataset. Your next challenge is to build a RESTful API using Node.js framework that will interfaces with the private blockchain.

By configuring an API for your private blockchain you expose functionality that can be consumed by several types of web clients ranging from desktop, mobile, and IoT devices. For your next project, you will be creating a RESTful web API for your private blockchain. The API project will require two endpoints:

- GET block
- POST block

## Why this project?

This project introduces you to the fundamentals of web APIs with Node.js frameworks. Using your own private blockchain to create a web API is a huge first step toward developing your own web applications that are consumable by a variety of web clients. Later in this program, you’ll be programming blockchain technologies that utilize these similar features using smart contracts.

## What will I learn?

You will learn to create and manage a web API with a Node.js framework to interact with your private blockchain. You’ll get first hand experience generating API endpoints and configuring the endpoints response that can be consumable by many types of web clients. This project helps build on the skills you’ve learned so far an allow you to apply these skills using real world technologies to get hands on with the tools used to create web APIs.

## How does this help my career?

Understanding web APIs and ways to create them will help you build user applications later in the program. These applications will serve as great portfolio items for potential employers.

## Project Prerequisites

Your project will be evaluated using the [Project Rubric](https://review.udacity.com/#!/rubrics/1707/view). For a project to pass, all criteria must “Meets Specifications”. Please thoroughly read through the rubric before beginning to build your project.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Installing Node and NPM is pretty straightforward using the installer package available from the (Node.js® web site)[https://nodejs.org/en/].

### Configuring your project

- Use NPM to initialize your project and create package.json to store project dependencies.
```
npm init
```
- Install crypto-js with --save flag to save dependency to our package.json file
```
npm install crypto-js --save
```
- Install level with --save flag
```
npm install level --save
```
- Install Express with --save flag
```
npm install express --save
```

## Testing

Run the server using
```
node index.js
```

GET /block/{BLOCK_HEIGHT}
example using curl:

POST /block
example using curl:
        curl -X POST http://localhost:8000/block -H 'Content-Type: application/json' -d $'{"body":"Test Block 1"}'

- Get Block Endpoint

http://localhost:8000/block/[blockheight]

For example using curl:
```
curl http://localhost:8000/block/0
```

The response for the endpoint should provide block object is JSON format.

- POST Block Endpoint

http://localhost:8000/block
example using curl:
```
curl -X POST http://localhost:8000/block -H 'Content-Type: application/json' -d $'{"body":"Test Block 1"}'
```

Several tools are available on the internet to assist with API development and testing. If you're having troubles testing your endpoints, try one of the tools listed below:

- Postman is a powerful tool used to test web services. It was developed for sending HTTP requests in a simple and quick way.
- CURL is a command-line tool used to deliver requests supporting a variety of protocols like HTTP, HTTPS, FTP, FTPS, SFTP, and many more.
