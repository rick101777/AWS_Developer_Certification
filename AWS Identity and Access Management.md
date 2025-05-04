Manage access in AWS by creating policies and attaching them to [[IAM]] identities (users, groups of users, or roles) or AWS Resources.

**Policy** - is an object in AWS that, when associated with an identity or resource, defines their permissions

#### Policy Types
The following policy types, listed in order from most frequently used to less frequently used, are available for use in AWS.

- **[[Identity-Based Policies]]**
	- Attach managed and inline policies to IAM identities. Identity-based policies grant permissions to an identity
- **[[Resource-Based Policies]]**
	- Attach inline policies to resources. 
	- The most common examples of resources-based policies are [[Amazon S3]] bucket policies and [[IAM]] role trust policies. 
	- Resource-based policies grant permissions to the principal that is specified in the policy. 
	- Principals can be in the same account as the resource or in other accounts
- **[[Permissions Boundaries]]**
	- Use the managed policy as the permissions boundary for an [[IAM]] entity (user or role)
	- That policy defines the maximum permissions that the identity-based policies can grant to an entity, but does not grant permissions
	- Permissions boundaries do not define the maximum permissions that a resource-based policy can grant to an entity
- **[[AWS Organizations SCPs]]**
	- Use an AWS Organizations service control policy (SCP) to define the maximum permissions for [[IAM]] users and [[IAM]] roles within accounts in your organization or organizational unit.
	- SCPs limit permissions that identity-based policies or resource-based policies grant to [[IAM]] users or [[IAM]] roles within the account
	- SCPs do not grant permissions
- **[[AWS Organizations RCPs]]**
	- Use an AWS Organizations resource control policy (RCP) to define the maximum permissions for resources within accounts in your organization or organizational unit
	- RCPs limit permissions that identity-based and resource-based policies can grant to resources in accounts within your organization
	- RCPs do not grant permissions
- **[[Access Control Lists]]**
	- Use ACLs to control which principals in other accounts can access the resource to which the ACL is attached
	- ACLs are similar to resource-based policies, although they are the only policy type that does not use the [[JSON Policy Document Structure]]
	- ACLs are cross-account permissions policies that grant permissions to the specified principal
	- ACLs cannot grant permissions to entities within the same account
- **[[Session Policies]]**
	- Pass advanced session policies when you use the [[AWS CLI]] or [[AWS API]] to assume a role or a federated user
	- Sessions policies limit the permissions that the role or user's identity-bases policies grant to the session
	- Session policies limit permissions for a created session, but do not grant permissions