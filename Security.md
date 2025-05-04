#### Task 1: Implement Authentication and/or Authorization for Applications and AWS Services

**Knowledge of:**
- [[Identity federation]]
	- [[Security Assertion Markup Langage]] (SAML)
	- [[OpenID Connect]] (OIDC)
	- [[Amazon Cognito]]
- [[Bearer Tokens]]
	- JSON Web Token (JWT)
	- OAuth
	- AWS Security Token Service (AWS STS)
- The comparison of user pools and identity pools in [[Amazon Cognito]]
- [[Resource-Based Policies]], [[Service Policies]], and [[Principal Policies]]
- [[Role-Based Access Controls]] (RBAC)
- Application authorization that uses ACLs
- The [[Principle of Least Privilege]]
- Differences between [[AWS Managed Policies]] and [[Customer-Managed Policies]]
- [[AWS Identity and Access Management (IAM)]]

**Skills In:**
- Using an identity provider to implement federated access
- Securing applications by using bearer tokens
- Configuring programmatic access to AWS
- Making authenticated calls to AWS Service
- Assuming an IAM Role
- Defining permissions for principals

#### Task 2: Implement Encryption by Using AWS Services

**Knowledge Of:**
- Encryption at rest and in transit
- [[Certificate Management]]
	- AWS Private Certificate Authority
- [[Key Protection]] (Key Rotation)
- Differences between [[Client-Side Encryption]] and [[Server-Side Encryption]]
- Differences between [[AWS Managed]] and [[Customer Managed]] [[AWS Key Management Service (AWS KMS)]] keys

**Skills In:**
- Using encryption keys to encrypt or decrypt data
- Generating certificates and SSH keys for development purposes
- Using encryption across account boundaries
- Enabling and Disabling Key Rotations

#### Task 3: Management Sensitive Data in Application Code

**Knowledge Of:**
- [[Data Classification]]
	- [[Personally Identifiable Information]] (PII)
	- [[Protected Health Information]] (PHI)
- [[Environment Variables]]
- [[Secrets Management]]
	- [[AWS Secrets Manager]]
	- [[AWS Systems Manager]] parameter store
- [[Secure Credential Handling]]

**Skills In:**
- Encrypting environment variables that contain sensitive data
- Using secret management services to secure sensitive data
- Sanitizing sensitive data