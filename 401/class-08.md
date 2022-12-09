[Home](../README.md)

# Class 8

## Role-based Access Control (RBAC)

### 5 Steps to RBAC

- RBAC refers to assigning people or systems roles and granting specific permissions based on their role, rather than granting permissions ona per-user basis. This is simpler, but also less flexible and granular than some other methods of access control
- A potential hierarchy could by Admin, Moderator, User, where each role has different permissions for crud operations on various routes or systems.

1. Inventory your systems
2. Analyze your workforce and and create roles
3. Assign people to roles
4. Never make one-off changes
5. Audit

### Wiki - RBAC

- Authentication is "you are who you say you are", and authorization is "you are allowed to go/access where/what you are trying to go/access"

#### Three Rules: ([from wiki page](https://en.wikipedia.org/wiki/Role-based_access_control))

  1. Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.
  2. Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
  3. Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.

- RBAC is basically the process of creating a table that outlines which types of users can do or access which things in the system, and then assigning all members of the system to a role.

### RBAC Tutorial

- Access rights are associated with the user's role(s), not the user.
- Access rights are activated after a user assumes a role, and after the user authenticates.
- RBAC can benefit a business by simplifying the process of granting or revoking permissions to a system, or making batch changes to which types of users can access what. It can also help with legal compliance due to its lack of flexibility.
