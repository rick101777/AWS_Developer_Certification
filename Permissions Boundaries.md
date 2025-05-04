A permissions boundary is an advanced feature in which you set the maximum permissions that an identity-based policy can grant to an [[IAM]] entity
- When you set a permissions boundary for an entity, the entity can perform only the actions that are allowed by its identity-based policies and its permissions boundaries
- If you specify a role session or user in the principal element of a resource-based policy, an explicit allow in the permission boundary is not required
- If you specify a role ARN in the principal element of a resource-based policy, an explicity allow in the permission boundary is required
- In Both cases, an explicit deny in the permission boundary is effective 
- An explicit deny in any of these policies overrides the allow
