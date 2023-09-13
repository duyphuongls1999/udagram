# Udagram

This application is provided to you as an alternative starter project if you do not wish to host your own code done in the previous courses of this nanodegree. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

## Project Overview
This project is simple application that includes angular front-end for user and backend to provide API.

The main feature of this project is:

- Login
- Add new feeds
- View feeds

## Getting Started
1. Clone this repo locally into the location of your choice
2. Move the content of the udagram folder at the root of the repository as this will become the main content of the project.
3. Open the terminal and navigate to the root of the repo
4. Follow the instructions in the Project Setup

The project can run but is missing some information to connect to the database and storage service

## Project Link
Frontend: http://udagram-frontend-last.s3-website-us-east-1.amazonaws.com/

Backend: http://udagram-api-last.eba-ipgvrked.us-east-1.elasticbeanstalk.com

## Project Setup
1. Download file udagram.zip and unzip file
2. Build & Run Frontend
   1. Go into the project directory - `cd udagram/udagram-frontend`
   2. Install the dependencies - `npm install`
   3. Start the frontend - `npm run start`
3. Build & Run Backend
   1. Go into the project directory - `cd udagram/udagram-api`
   2. Setup environment depend on `set_env.sh`
   3. Install the dependencies - `npm install`
   4. Start the backend - `npm run dev`
4. In AWS, provision a publicly available RDS database running Postgres.
5. In AWS, provision a s3 bucket for hosting the uploaded files.
6. Setup ENV variables:

```
export POSTGRES_USERNAME=postgres     // Postgres username
export POSTGRES_PASSWORD=postgres     // Postgres password
export POSTGRES_HOST=''               // Postgres Host
export POSTGRES_DB=postgres           // Database name
export AWS_BUCKET=udagram-frontend-last    // S3 bucket
export AWS_REGION=us-east-1           // AWS region
export AWS_PROFILE=default            // AWS profile
export JWT_SECRET=mysecret      // JWT secret key
```

## Documentation

- Detailed Documentation is provided in `./docs/README.md`
- Screenshots of the AWS configurations and the CircleCI are provided in `./docs/screenshots/`
- Architecture Diagrams of the AWS and the Pipeline are provided in `./docs/architecture/`

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework
