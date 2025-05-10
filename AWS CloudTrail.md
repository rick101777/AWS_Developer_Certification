AWS CloudTrail is an AWS service that helps you enable operational and risk auditing, governance, and compliance of your AWS account
- Actions taken by a user, role, or an AWS service are recorded as events in CloudTrail
- Event include actions taken in the AWS management console, AWS command line interface, and AWS SDKs and APIs

CloudTrail provides three ways to record events:
- **Event History**
	- The event history provides a viewable, searchable downloadable, and immutable record of the past 90 days of management events in an AWS Region
	- You can search events by filtering on a single attribute
	- You automatically have access to the event history when you create your account
- **CloudTrail Lake**
	- AWS CloudTrail Lake is managed data lake for capturing, storing, accessing, and analyzing user and API activity on AWS for audit and security purposes
	- CloudTrail Lake coverts existing events in row-based JSON format to Apache ORC format
	- ORC is a columnar storage form that is optimized for fast retrieval of data
	- Events are aggregated into event data stores, which are immutable collections of events based on criteria that you select by applying advanced event selectors
	- You can keep the even data in an event data store for up to 3,653 days(about 10 years) if you choose the One-year extendable retention pricing option, or up to 2,557 days (about 7 years) if you choose the 7 year option
	- You can create an event data store for a single AWS account or for multiple AWS accounts by using AWS Organizations
	- You can import any existing CloudTrail logs from your S3 buckets into an existing or new event data store
	- You can also visualize top CloudTrail event trends with Lake dashboards
- **Trails**
	- Trails capture a record of AWS activities, delivering and storing these events in an Amazon S3 bucket, with optional delivery to [[Amazon CloudWatch]] Logs and [[Amazon EventBridge]]
	- You can input these events into your security monitoring solutions
	- You can also use your own third-party solutions or solutions such as [[Amazon Athena]] to search and analyze your CloudTrail logs
	- You can create trails for a single AWS account or for multiple AWS account by using AWS Organizations
	- You can log insights events to analyze your management event for anomalous behavior in API call rates and error rates
	- You can deliver one copy of your ongoing management events to your S3 bucket at no charge from CloudTrail by creating a trail however, there are [[Amazon S3]] storage charges

#### Access CloudTrail
You can work with CloudTrail in any of the following ways:
- CloudTrail console
- AWS CLI
- CloudTrail APIs
- AWS SDK

#### CloudTrail Console
Sign in to the AWS Management Console and open the CloudTrail console

The CloudTrail console provides a user interface for performing many CloudTrail tasks such as:
- Viewing recent events and event history for your AWS account
- Downloading a filtered or complete file of the last 90 days of management events from Event history
- Creating and editing CloudTrail trails
- Creating and editing CloudTrail Lake event data stores
- Running queries on event data stores
- Configuring CloudTrails trails, including:
	- Selecting an [[Amazon S3]] bucket for trails
	- Setting a prefix
	- Configuring delivery to [[Amazon CloudWatch]] Logs
	- Using [[AWS Key Management Service (KMS)]] keys for encryption of trail data
	- Enabling [[Amazon Simple Notification Service (SNS)]] notifications for log file delivery on trails
	- Adding and managing tags for your trails
- Configuring CloudTrail Lake event data stores, including:
	- Integrating event data stores with CloudTrail partners or with your own applications, to log events from sources outside of AWS
	- Federating event data stores to run queries from [[Amazon Athena]]
	- Using [[AWS Key Management Service (KMS)]] keys for encryption of event data store data
	- Adding and managing tags for your event data stores
#### AWS CLI
The AWS Command Line Interface is a unified tool that you can use to interact with CloudTrail from the command line.

#### CloudTrail APIs
In addition to the console and the CLI, you can also user the CloudTrail RESTful APIs to program CloudTrail directly

#### AWS SDKs
As an alternative to using the CloudTrail API, you can use one of the AWS SDKs.
- Each SDK consists of libraries and sample code for various programming languages and platforms
- The SDKs provide a convenient way to create programmatic access to CloudTrail