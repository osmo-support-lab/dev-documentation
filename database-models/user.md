# User

### Description

The user represents organisation admins and agents. A user is global and can belong to multiple organisations. In the first version a User will not be able to create tickets and request support. This functionality shall be implemented at a later stage.

### Attributes

| Attribute | Type   | Description                   |
| --------- | ------ | ----------------------------- |
| user\_id  | int    | User id identifying the user. |
| username  | string |                               |
| email     | string |                               |
| password  | string | argon2 hashed password        |
| avatar    | string | avatar url on our CDN         |

### Relations
