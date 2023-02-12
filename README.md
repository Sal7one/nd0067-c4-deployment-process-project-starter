
# Hosting a Full-Stack Application


### Architecture

<img src="documentation/architechture_diagram.jpg" alt="drawing" width="600"/>


<br>

### Deployment Pipeline
<img src="screenshot/pipeline.png" alt="drawing" width="600"/>

1 - Circle CI Gets Notify by version control on new project verison then Builds the Project and runs test scripts

2 - Circle CI Then Holds and waits for apporval if granted it will start deploying 

3 - in Deployment Cricle Ci deploys an elastic beanstalk for the backend and stores the frontend files in an S3 bucket

## LIVE URL (Frontend)

<a href="http://salehsubmissionbuckets.s3-website-us-east-1.amazonaws.com/"> Frontend</a>

## LIVE URL (Backend)

<a href="http://salehsubmission-dev.us-east-1.elasticbeanstalk.com/api/v0"> Backend</a>



## Screen Shots 

<img src="screenshot/circlecibuild.png" alt="drawing" width="600"/>
<img src="screenshot/deploy.png" alt="drawing" width="600"/>
<img src="screenshot/ENVVARS.png" alt="drawing" width="600"/>
<img src="screenshot/eb.png" alt="drawing" width="600"/>
<img src="screenshot/s3.png" alt="drawing" width="600"/>
<img src="screenshot/rds.png" alt="drawing" width="600"/>


# Udagram

This application is provided to you as an alternative starter project if you do not wish to host your own code done in the previous courses of this nanodegree. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.



### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
