If you enable all features in an organization, then you can use resource control policies (RCPs) to centrally apply access controls on resources across multiple AWS accounts
- RCPs are JSON policies that you can use to set the maximum available permissions for resource in your accounts without updating the [[IAM]] policies attached to each resource that you own
- The RCP limits permissions for resources in member accounts and can impact the effective for identities, including the AWS account root user, regardless of whether they belong to your organization
- An explicit deny in any applicable RCP overrides an allow in other policies that might be attached to individual identities or resources
