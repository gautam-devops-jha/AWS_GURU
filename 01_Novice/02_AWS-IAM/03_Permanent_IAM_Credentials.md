# The Building Blocks of IAM

1. **USers** :- A physical person, one user should always be one human being.
2. **Groups** :- We should group our users into groups and this should be by job functions, such as administrator, DevOps, Developers, etc.
3. **Roles** :- Roles are for internal usage within AWS, It allow one part of allows to access another part of AWS. For example allowing our EC2 machines to use S3 buckets without AWS credentials. 


## Policy best practices 
- IAM policy should be attached to Groups and roles
- User must inherit the permission from group instead of policy directly attached with user.

## Users and People best practices
- Always work on principle that one user equals one physical person. Never share accounts across multiple people. 

## Principle of least privilege
- Only assign a user the minimum amount of previleges they need to do their job.


