# sqs-fargate-autoscaling
Fargate autoscaling based on the SQS depth

### Overview 
A Lambda polls the messages from the SQS and Launches a New Fargate Task whenever a message is available.

### Dependencies

Run the below command in the root directory to install the dependencies

`npm install`

### Requirements
- Docker
- Serverless
- AWS Credentials

### Dokcer

Run the below command to build the docker image 

`docker build --tag <<tagName>> . `

### Deployment

Run the below command in the root directory to deploy

`sls deploy --stage <<stageName>>`