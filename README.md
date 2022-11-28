#  GitHubActions
This repository contains GitHub actions to accomplish various tasks.

## Features

### deployLambda.yml
GitHub Action file to deploy the source code (index.js) to existing AWS Lambda

### updateCloudfront.yml 
GitHub Action to update the CloudFront (Origin request of Function Association) with latest Lambda@edge ARN. This function will trigger only if the previous action (updating the AWS Lambda) is successful

## Pre-requisites

The following secrets to be added in the GitHub repository:
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY

Add secrets to the Github Repository by following steps
```
GitHub Repository -> Settings -> Security -> Actions
```
