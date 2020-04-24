# SAM

## Overview

- framework for developing and deploying serverless apps
- all the configuration is YAML code
- generate complex CloudFormation from simple SAM YAML file
- can run Lambda, API Gateway, DynamoDB locally

## Recipe

- Transform Header indicates it's SAM template:
    - `Transform: 'AWS::Serverless-2016-10-31'`
- Write Code
    - `AWS::Serverless::Function`
    - `AWS::Serverless::Api`
    - `AWS::Serverless::SimpleTable`
- Package & Deploy:
    - `aws cloudformation package / sam package`
    - `aws cloudformation deploy / sam deploy`