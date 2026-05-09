# CDK Course Resources

This repository groups the projects built throughout the **AWS TypeScript CDK, Serverless & React** Udemy course.

## Projects

### [cdk-starter](https://github.com/jorgechavezrnd/cdk-starter)
A blank CDK TypeScript starter project used to learn the fundamentals of AWS CDK. Covers core CDK commands, CloudFormation stack synthesis, bootstrapping, and deploying stacks to AWS.

### [space-finder](https://github.com/jorgechavezrnd/space-finder)
A full CDK backend application built from scratch (without `cdk init`). Implements a REST API with AWS Lambda, DynamoDB, API Gateway, and Cognito authentication to manage spaces/locations.

### [space-finder-frontend](https://github.com/jorgechavezrnd/space-finder-frontend)
Frontend web application for the Space Finder project. Built to be deployed on AWS and integrated with the Space Finder backend services provisioned via AWS CDK.

## Cloning with Submodules

To clone this repository and download all submodules in a single command:
```bash
git clone --recurse-submodules https://github.com/jorgechavezrnd/CDK-course-resources.git
```

If you already cloned the repo and the submodules are empty, run:
```bash
git submodule update --init --recursive
```

## Updating Submodules

### Update all submodules to the latest changes
```bash
git submodule update --remote
git add .
git commit -m "Update submodules to latest"
git push
```

### Update a specific submodule only
```bash
git submodule update --remote space-finder
git add space-finder
git commit -m "Update space-finder submodule to latest"
git push
```

> **Note:** The three individual repos (`cdk-starter`, `space-finder`, `space-finder-frontend`) are not affected by these commands — you still push changes to them independently as usual. These commands only update the **pointer** in the parent repo to point to their latest commit.

## Resources

- 🎓 [Udemy Course — AWS TypeScript CDK, Serverless & React](https://www.udemy.com/course/aws-typescript-cdk-serverless-react/?couponCode=MT260504G1)
- 📦 [Original Course Repository](https://github.com/alexhddev/CDK-course-resources)
