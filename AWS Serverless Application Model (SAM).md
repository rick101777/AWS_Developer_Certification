AWS Serverless Application Model (SAM) is an open-source framework for building serverless applications using infrastructure as code (IAC).
- With SAM's shorthand syntax, developers declare [[AWS CloudFormation]] resources and specialized serverless resources that are transformed to infrastructure during deployment
- This framework includes two main components
	1. AWS SAM CLI
	2. AWS SAM Project
- The SAM Project is the application project directory that is created when you run `sam init`
- The SAM Project includes files like the SAM template, which includes the template specification

#### Key Features
AWS SAM offers a variety of benefits that improve the developer experience by allowing you to:

**Define your application infrastructure code quickly, using less code**
- Author AWS SAM templates to define your serverless application infrastructure code
- Deploy your templates directly to [[AWS CloudFormation]] to provision your resources

**Manage your serverless application through their entire development lifecycle**
- Use the AWS SAM CLI to manage your serverless application through the authoring, building, testing, and monitoring phases of your development lifecycle

**Quickly provision permissions between resources with AWS SAM connectors**
- Use SAM connector in your AWS SAM templates to define permissions between your AWS resources
- AWS SAM transforms your code into the [[AWS Identity and Access Management (IAM)]] permissions required to facilitate your intent

**Continuously sync local changes to the cloud as you develop**
- Use the AWS SAM CLI `sam sync` command to automatically sync local changes to the cloud, speeding up your development and cloud testing workflows

**Manage your Terraform serverless applications**
- Use the AWS SAM CLI to perform local debugging and testing of your [[AWS Lambda]] functions and layers

