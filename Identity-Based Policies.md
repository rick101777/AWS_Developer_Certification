Identity-based policies are JSON permissions policy documents that control what actions an identity can perform, on which resources, and under what conditions. Identity-based policies can be further categorized:

- **Managed Policies**
	- Standalone identity-based policies that you can attach to multiple users, groups, and roles in your AWS account. 
	- There are two types of managed policies
		- **AWS Managed Policies**
			- Managed Policies that are created and managed by AWS
		- **[[Customer-Managed Policies]]**
			- Managed policies that you create and manage in your AWS account
			- Customer managed policies provide more precise control over your policies than AWS managed policies
- **Inline Policies**
	- Policies that you add directly to a single user, group, or role
	- Inline policies maintain a strict one-to-one relationship between a policy and an identity
	- They are deleted when you delete the identity
