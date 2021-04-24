# Rust + AWS Lambda + ASW CDK 

## Overview
An overview of commands (all prefixed with `npm run`):

| Command | Description |
|---------|-------------|
| `build` | Build the Rust executable |
| `build:clean` | Cleans build artifcats from `target/cdk` |
| `deploy` | Cleans and builds a new executable, and deploys it via CDK |
| `cdk:bootstrap` | Bootstrap necessary resources on first usage of CDK in a region |
| `cdk:deploy` | deploy this stack to your default AWS account/region |
| `cdklocal:start` | Starts the LocalStack docker image |
| `cdklocal:bootstrap` | Bootstrap necessary resources for CDK against LocalStack |
| `cdklocal:deploy` | Deploy this stack to LocalStack |

## Usage

### build & deploy

1. npm run build
2. export AWS_REGION=<your target region>
3. npm run cdk:bootstrap
4. npm run deploy

### deploy localstack

1. export AWS_REGION=<your target region>
2. npm run cdklocal:start
3. npm run cdklocal:bootstrap
4. npm run cdklocal:deploy

