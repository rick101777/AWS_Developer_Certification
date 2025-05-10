CodeDeploy is a deployment service that automates application deployments to [[Amazon EC2]], on-premises instances, serverless [[AWS Lambda]] functions, or [[AWS Elastic Container Services (ECS)]]

You can deploy a nearly unlimited variety of application content, including:
- Code
- Serverless AWS Lambda Functions
- Executables
- Packages
- Scripts
- Multimedia files

CodeDeploy can deploy application content runs on a server and is stored in [[Amazon S3]] buckets, GitHub repositories, or Bitbucket repositories. CodeDeploy can also deploy a serverless Lambda function. You do not need to make changes to your existing code before you can use CodeDeploy.

CodeDeploy makes it easier for you to:
- Rapidly release new features
- Update AWS Lambda functions versions
- Avoid downtime during application deployment
- Handle the complexity of updating your application, without many of the risks associated with error-prone manual deployments

#### Benefits of AWS CodeDeploy
CodeDeploy offers these benefits
- **Serve, Serveless, and Container Applications**
	- CodeDeploy lets you deploy both traditional applications on servers and application that deploy a serverless [[AWS Lambda]] function version or an [[AWS Elastic Container Services (ECS)]] application
- **Automated Deployment**
	- CodeDeploy fully automates your application deployments across your development, test, and production environments
	- CodeDeploy scales wit your infrastructure so that you can deploy to one instance or thousands
- **Minimize Downtime**
	- If you application uses the EC2/On-Premises compute platform, CodeDeploy helps maximize your application availability
	- During an in-place deployment, CodeDeploy performs a roiling update across [[Amazon EC2]] instances
	- You can specify the number of instances to be taken offline at a time for updates
	- During a [[Blue/Green]] deployment, the latest application revision is installed on replacement instances
	- Traffic is rerouted to these instances when you choose, either immediately or as soon as you are done testing the new environment
	- For both deployment types, CodeDeploy tracks application health according to rules you configure
- **Stop and Rollback**
	- You can automatically or manually stop and roll back deployments if there are errors
- **Centralized Control**
	- You can launch and track the status of your deployments through the CodeDeploy console or the [[AWS CLI]]
	- You receive a report that lists when each application revision was deployed and to which [[Amazon EC2]] instances
- **Easy to Adopt**
	- CodeDeploy is platform-agnostic and works with any application
	- You can easily reuse you setup code
	- CodeDeploy can also integrate with your software release process or continuous delivery toolchain
- **Concurrent Deployments**
	- If you have more than one application that uses EC2/On-Premises compute platform, CodeDeploy can deploy them concurrently to the same set of instances


#### Overview of CodeDeploy Compute Platforms


#### Overview of CodeDeploy Deployment Types
CodeDeploy provides two deployment type options:
- **In-Place Deployment**
	- The application on each instance in the deployment group is stopped, the latest application revision is installed, and the new version of the application is started and validated
	- You can use a load balancer so that each instance is deregistered during its deployment and then restored to service after the deployment is complete
	- Only deployments that use the EC2/On-Premises compute platform can use in-place deployments
- **Blue/Green Deployment**
- The behavior of your deployment depends on which compute platform you use
	- **Blue/Green on an EC2/On-Premises Compute Platform**
		- The instances in a deployment group (the original environment) are replaced by a different set of instances (the replacement environment) using these steps:
			- Instances are provisioned for the replacement environment
			- The latest application revision is installed on the replacement instances
			- An optional wait time occurs for activities such as application testing and system verification
			- Instances in the replacement environment are registered with one or more [[Elastic Load Balancing (ELB)]], causing traffic to be rerouted to them
				- Instances in the original environment are deregistered and can be terminated or kept running for other uses
	- **Blue/Green on an AWS Lambda or Amazon ECS Compute Platform**
		- Traffic is shifted in increments according to a [[Canary]], [[Linear]], or [[All-At-Once]] deployment configuration
	- **Blue/Green Deployments Through [[AWS CloudFormation]]**
		- Traffic is shifted from your current resources to your updated resources as part of an [[AWS CloudFormation]] stack update
		- Currently, only [[AWS Elastic Container Services (ECS)]] [[Blue/Green]] deployments are supported


