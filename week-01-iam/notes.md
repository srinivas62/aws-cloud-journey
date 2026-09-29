# Week 1 - IAM Notes

## What is IAM?
IAM (Identity and Access Management) controls WHO can access WHAT in AWS.

## Key concepts
- **User**: represents a person or application, has long-term credentials
- **Group**: a collection of users that share the same permissions
- **Role**: temporary permissions that can be "assumed" by a user, service, or app (e.g. EC2 assuming a role to access S3)
- **Policy**: a JSON document that defines permissions (Allow/Deny on specific actions/resources)

## Key rule
Everything is denied by default. Permissions must be explicitly granted.
An explicit Deny always overrides an Allow.

## Best practice
Never use the root account for daily work. Use IAM users/roles with least privilege.