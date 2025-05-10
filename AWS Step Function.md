With AWS Step Functions, you can create workflows, also called [[State Machines]], to build distributed applications, automate processes, orchestrate micoservices, and create data and machine learning pipelines

Step Functions is based on [[State Machines]] and [[Tasks]]. 
- In Step Functions, state machines are called [[Workflows]], which are a series [[Event Driven]] steaps
- Each step in a [[Workflows]] is called [[State]]

The work of your [[State Machines]] tasks can also be done using [[Activities]] which are workers that exist outside of Step Functions

![[Pasted image 20250504205739.png]]
#### Standard and Express Workflows Types
Step Functions has two workflow types
- **Standard**
	- Workflows are ideal for long-running, auditable workflows, as they show execution history and visual debugging
	- Standard workflows have exactly-once workflow execution and can run for up to one year
	- This means that each step in a Standard workflow will execute exactly once
- **Express**
	- Workflows are ideal for high-event-rate workloads, such as streaming data processing and IoT data ingestion
	- Express workflows have at-least-once workflow execution and can run for up to five minutes
	- This means that one or more steps in an Express Workflow can potentially run more than once, while each step in the workflow executes at least once


| Standard Workflows                                                                                                                | Express Workflows                                              |
| --------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 2,000 per second execution rate                                                                                                   | 100,000 per second execution rate                              |
| 4,000 per second state transition                                                                                                 | Nearly unlimited state transition rate                         |
| Priced by state transition                                                                                                        | Priced by number and duration of executions                    |
| Show execution history and visual debugging                                                                                       | Show execution history and visual debugging based on log level |
| See execution history in Step Functions                                                                                           | Send execution history to [[Amazon CloudWatch]]                |
| Support integration with all services<br><br>Support optimized integrations with some services                                    | Support integrations with all services                         |
| Support Request Response pattern for all services<br><br>Support Run a Job and/or Wait For Callback patterns in Specific services | Support Request Response pattern for all services              |
#### Integrating with Other Services
Step Functions integrates with multiple AWS services. To call other AWS services, you can use two integration types
- **AWS SDK Integrations**
	- Provides a way to call any AWS service directly from your [[State Machines]], giving you access to thousands of API actions
- **Optimized Integrations**
	- Provide custom options for using those services in your [[State Machines]]

To combine Step Functions with other services, there are three service integration patterns
- **Request Response**
	- Call a service and let Step Functions progress to the next state after it gets an HTTP response
- **Run a Job (.sync)**
	- Call a service and have Step Functions wait for a job to complete
- **Wait for a Callback with a Task Token (.waitForTaskToken)**
	- Call a service with a task token and have Step Functions wait until the task token returns with a callback

Standard Workflows and Express Workflows support the same integrations but not the same integration patterns
- **Standard Workflows**
	- support Request Response integrations
	- Certain services support Run a Job or Wait for Callback
- **Express Workflows**
	- Only support Request Response

![[Pasted image 20250510110451.png]]