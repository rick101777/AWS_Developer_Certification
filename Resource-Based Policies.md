Resource-based policies are JSON policy documents that you attach to a resource such as an [[Amazon S3]] bucket. 
- These policies grant the specified principal permission to perform specific actions on that resource and defines what conditions this applies. 
- Resource-based policies are inline policies. 
- There are not managed resource-based policies

To enable cross-account access, you can specify an entire account or [[IAM]] entityies in another account as the principal in the resource-based policy
- Adding a cross-account principal to a resource-based policy is only half of establishing the trust relationship
- When the principal and the resource are in separate AWS accounts, you must also use an identity-based policy to grant the principal access to the resource
- If a resource-based policy grants access to a principal in the same account, no additional identity-based policy is required


The [[IAM]] service supports only one type of resource-based policy called a role [[Trust Policy]], which is attached to an [[IAM]] role.
- An [[IAM]] role is both an identity and a resource that supports resource-based policies
- You must attach both a [[Trust Policy]] and an identity-based policy to an [[IAM]] role
- [[Trust Policy]] define which principal entities (accounts, users, roles, and federated users) can assume the role