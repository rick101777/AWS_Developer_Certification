AWS Lambda is a serverless compute service.

**Features:**
- Lambda executes code only when needed and scales automatically
- Lambda functions are [[Stateless]]
- Memory can be specifically allocated
	- Proportional CPU, network bandwidth and disk I/O will be allocated
- Natively supports the following languages
	- Node.js
	- Java
	- C#
	- Go
	- Python
	- Ruby
	- PowerShell
- Can provide a custom runtime

#### Components of a Lambda Application

- **Function** - a script or program that runs in Lambda. Lambda passes invocation events to you function. The function processes an event and returns a response.
- **Execution environment** - a secure, isolated micro virtual machine where a Lambda function is executed
- **Runtimes** - Lambda runtimes allow functions in different languages to run in the same base execution environment. The runtime sits in-between the Lambda service and your function code, relaying invocation events, context information, and response between the two
- **Environment Variables** - key-value pairs that you can use to store configuration settings for your function.
- **Layers** - Lambda layers are a distributed mechanism for libraries, custom runtimes, and other function dependencies. Layers let you manage your in-development function code independently from the unchanging code and resources that it uses
- **Event Source** - An AWS service or a custom service that triggers your function and executes its logic
- **Downstream Resources** - An AWS service that your Lambda function calls once it is triggered
- **Log Streams** - While Lambda automatically monitors your function invocations and reports metrics to [[CloudWatch]], you can annotate your function code with custom logging statements that allow you to analyze the execution flow and performance of you Lambda function
- AWS Serverless Application Model

#### Lambda Functions
- You can upload your application code as a ZIP file or a container hosted on AWS [[Elastic Container Registry (ECR)]]
- To create a Lambda function, you first package your code and dependencies in a deployment package. Then, you upload the deployment package to create your Lambda function
- After your Lambda function is in production, Lambda automatically monitors functions on your behalf, reporting metrics through [[CloudWatch]]

Configure basic function settings
- Description
- Memory Usage (512MB - 10 GB)
- Execution Timeout (15 min max)
- IAM Role

- Environment variables are always encrypted at rest and can be encrypted in transit as well
- Versions - a snapshot of your function's state at a given time.
	- When you publish a new version, a version number is appended to your functions ARN
	- arn:aws:lambda:us-east-2:123456789123:function:my-function:1
- Aliases - serves as a pointer to a Lambda function version. Aliases create a human readable version of the function's name, making it easier to remember and understand what the function does.
	- - arn:aws:lambda:us-east-2:123456789123:function:my-function:MyAlias
- A layer is a ZIP archive that contains libraries, a custom runtime, or other dependencies. Use layers to manage your function's dependencies independently and keep your deployment package small
- You can configure a function to mount an Amazon [[Elastic File System (EFS)]] file system to a local directory. With [[Elastic File System (EFS)]], your function code can access and modify shared resources securely and at high concurrency

#### Invoking Lambda Functions
