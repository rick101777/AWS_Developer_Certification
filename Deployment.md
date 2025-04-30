#### Task 1: Prepare Application Artifacts to be Deployed to AWS

**Knowledge Of:**
- Ways to access [[Application Configuration]] data
	- [[AppConfig]]
	- [[Secrets Manager]]
	- [[Parameter Store]]
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
- [[API Gateway]] Stages
- Branches and actions in the [[Continuous Integration and Continuous Delivery (CI/CD)]] workflow
- Automated Software Testing
	- Unit Testing
	- Mock Testing

**Skills In:**
- Creating application test events
	- JSON payload for testing Lambda
	- API Gateway
	- AWS SAM resources
- Deploying API resources to various environments
- Creating application environments that use approved versions for integration testing
	- Lambda Aliases
	- Container Image Tags
	- AWS Amplify Branches
	- AWS Copilot environments
- Implementing and deploying infrastructure as code (IaC) templates
	- AWS SAM Templates
	- AWS CloudFormation Templates
- Managing environment in individual AWS services
	- Development, test, production in API Gateway


#### Task 4: Deploy Code by Using AWS CI/CD Services

**Knowledge Of:**
- Git-based version control tools
- Manual and Automated approvals in AWS [[Code Pipeline]]
- Access application configurations from AWS [[AppConfig]] and [[Secrets Manager]]
- CI/CD workflows that use AWS Services
- Application deployment that use AWS services and tools
	- [[CloudFormation]]
	- [[Cloud Development Kit]] (CDK)
	- [[SAM]]
	- [[CodeArtifact]]
	- [[Copilot]]
	- [[Amplify]]
	- [[Lambda]]
- Lambda deployment packaging options
- [[API Gateway]] stages and custom domains
- [[Deployment strategies]]
	- [[Canary]]
	- [[Blue/Green]]
	- [[Rolling]]

