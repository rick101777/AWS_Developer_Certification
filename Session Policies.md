Session policies are advanced policies that you pass as a parameter when you programmatically create a temporary session for a role or federated users
- The permissions for a session are the intersection of the identity-based policies for the [[IAM]] entity used to create the session and the session policies
- Permissions can also come from a resource-based policy
- An explicit deny in any of these policies overrides the allow

You can create role session and pass session policies programmatically using the AssumeRole, AssumeRoleWithSAML, or AssumeRoleWithWebIdentity API operations
- You can pass a single JSON inline session policy document using the Policy parameter
- You can use the PolicyArns parameter to specify up to 10 managed session policies

When you create a federated user session, you use the access keys of the [[IAM]] user to programmatically call the GetFederationToken API operation
- You must also pass session policies
- The resulting session's permissions are the intersection of the identity-based policies and the session policy

