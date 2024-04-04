# How do we control permissions using IAM?
We assign permissions using policy documents, which are made up of JSON (JavaScript Object Notation).

## Example of policy document

```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": "*",
            "Resource": "*"
        }
    ]
}
```

So we got the version and then we've got the statement itself and then inside the statement, we've got a number of different key pairs. So we got effect which is allow. So basically we're allowing the action is what and then it's a wild card. so we are allwing everything and the resource is wild card as well. So it's that just simply means everything. 

So this is the full adminstrator access. The json is saying allow the action of everything on every resource.

This allows the person who this policy documents attached to or the group that this policy documents attached to the ability to do everything with every resource. 

## IAM Policy Documents can be assigned to
- Groups
- Users
- Roles 


