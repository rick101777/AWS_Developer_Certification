AWS CloudFormation allows you to create and manage AWS infrastructure deployments predictably and repeatedly. You can use CloudFormation to leverage AWS products, such as [[Amazon EC2]], [[Amazon Elastic Block Store (EBS)]], [[Amazon Simple Notification Service (SNS)]], [[Elastic Load Balancing (ELB)]], and [[Amazon EC2]] Auto Scaling to build highly reliable, highly scalable, cost effective applications without creating or configuring the underlying AWS infrastructure

With CloudFormation, you declare all your resources and dependencies in a template file
- The template defines a collection of resources as a single unit called a **Stack**
- CloudFormation creates and deletes all member resources of the stack together and manages all dependencies between the resources for you

#### Stack Actions
- When you use CloudFormation, you manage related resources as a single unit called a Stack. 
- You create, update, and delete a collection of resources by creating, updating and deleting stacks. 
- All the resources in a stack are defined by the stack's template

Stack Actions: https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_Operations.html
