#### Task 1: Prepare Application Artifacts to be Deployed to AWS

**Knowledge Of:**
- Ways to access [[Application Configuration]] data
	- [[AWS AppConfig]]
	- [[AWS Secrets Manager]]
	- [[AWS Parameter Store]]
- Lambda deployment packaging, layers, and configuration options
- Git-based version control tools
- Container Images

**Skills In:**
- Managing the dependencies of the code module
	- Environment variables
	- Configuration files
	- Container images
- Organizing files and a directory structure for application deployment
- Using code repositories in deployment environment
- Applying application requirements for resources

#### Task 2: Test Application in Development Environments

**Knowledge Of:**
- Features in AWS Services that perform application deployment
- [[Integration Testing]] that uses mock endpoints
- [[Lambda Versions and Aliases]]

**Skill In:**
- Testing deployed code by using AWS services and tools
- Performing mock integration for APIs and resolving integration dependencies
- Testing applications by using development endpoints
	- API Gateway
- Deploying application stack updates to existing environments
	- AWS SAM Template to a different staging environment

### Task 3: Automate Deployment Testing

**Knowledge Of:**
- [[Amazon API Gateway]] Stages
- Branches and actions in the [[Continuous Integration and Continuous Delivery (CI/CD)]] workflow
- Automated Software Testing
	- Unit Testing
	- Mock Testing

**Skills In:**
- Creating application test events
	- JSON payload for testing Lambda
	- API Gateway
	- [[AWS Serverless Application Model (SAM)]] resources
- Deploying API resources to various environments
- Creating application environments that use approved versions for integration testing
	- Lambda Aliases
	- Container Image Tags
	- [[AWS Amplify]] Branches
	- [[AWS Copilot]] environments
- Implementing and deploying infrastructure as code (IaC) templates
	- [[AWS Serverless Application Model (SAM)]] Templates
	- [[AWS CloudFormation]] Templates
- Managing environment in individual AWS services
	- Development, test, production in [[Amazon API Gateway]]


#### Task 4: Deploy Code by Using AWS CI/CD Services

**Knowledge Of:**
- Git-based version control tools
- Manual and Automated approvals in [[AWS CodePipeline]]
- Access application configurations from [[AWS AppConfig]] and [[AWS Secrets Manager]]
- CI/CD workflows that use AWS Services
- Application deployment that use AWS services and tools
	- [[AWS CloudFormation]]
	- [[AWS Cloud Development Kit (AWS CDK)]]
	- [[AWS Serverless Application Model (SAM)]]
	- [[AWS CodeArtifact]]
	- [[AWS Copilot]]
	- [[AWS Amplify]]
	- [[AWS Lambda]]
- Lambda deployment packaging options
- [[Amazon API Gateway]] stages and custom domains
- [[Deployment strategies]]
	- [[Canary]]
	- [[Blue/Green]]
	- [[Rolling]]

