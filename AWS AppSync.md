AWS AppSync enables developers to connect their applications and services to data and events with secure, serverless and high performing GraphQL, and Pub/Sub APIs. 

You can do the following with AWS AppSync
- Access data from one or more data sources from a single GraphQL API endpoint
- Combine multiple source GraphQL APIs into a single, merged GraphQL API
- publish real-time data updates to your application
- Leverage built-in security, monitoring, logging, and tracing, with optional caching for low latency
- Only pay for API requests and any real-time messages that are delivered

#### App Sync Features
- Simplified data access and querying, powered by GraphQL
- Serverless WebSockets and GraphQL subscriptions and pub/sub channels
- Server-side caching to make data available in high speed in-memory caches for low latency
- JavaScript and TypeScript support to write business logic
- Enterprise security with Private APIs to restrict API access and integration with [[AWS WAF]]
- Built in authorization controls, with support for API keys, [[AWS Identity and Access Management (IAM)]], [[Amazon Cognito]], [[OpenID Connect]] providers, and [[AWS Lambda]] authorization for custom logic
- Merged APIs to support federated use cases

#### Pricing for AWS AppSync
AWS AppSync is priced based on millions of requests and updates. Caching costs an additional fee

The following lists the exceptions to general AWS AppSync pricing
- API caching in AWS AppSync is not eligible for the AWS free tier
- Requests are not charged for authorization and authentication failures
- Calls to methods that require API keys are not charged when API keys are missing or invalid
