As illustrated in the following figure, a JSON policy document includes these elements
- Optional policy-wide information at the top of the document
- One or more individual statements

Each statement includes information about a single permission. If a policy includes multiple statements, AWS applies a logical OR across the statements when evaluating them. If multiple policies apply to a request AWS applies a logical OR across all of those policies when evaluating them

![[Pasted image 20250504123715.png]]
A statement contains a series of elements:
- **Version**
	- Specify the version of the policy language that you want to use
	- We recommend that you use the latest `2012-10-17` version
- **Statement**
	- Use the main policy element as a container for the following elements
	- You must include more than one statement in a policy
- **Sid (Optional)**
	- Include an optional statement ID to differentiate between your statements
- **Effect**
	- Use `Allow` or `Deny` to indicate whether the policy allows or denies access
- **Principal**
	- (Required in some circumstances) if you create a resource-based policy, you must indicate the account, user, role, or federated user to which you would like to allow or deny access
	- If you are creating an [[AWS Identity and Access Management (IAM)]] permissions policy to attach to a user or role, you cannot include this element
	- The principal is implied as that user or role
- **Action**
	- Include a list of actions that the policy allows or denies
- **Resource**
	- (Required in some circumstances) If you create an [[AWS Identity and Access Management (IAM)]] permissions policy, you must specify a list of resources to which the actions apply
	- If you create a resource-based policy, it depends on the resource you're using as to whether this element is required or not
- **Condition (Optional)**
	- Specify the circumstances under which the policy grants permission
