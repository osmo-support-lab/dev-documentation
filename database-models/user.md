# User

### Attributes

| Attribute      | Type   | Description                                                                                |
| -------------- | ------ | ------------------------------------------------------------------------------------------ |
| uuid           | uuid4  | User id identifying the user. For temp\_users this will also be their authentication token |
| is\_temp\_user | bool   | Whether a user registered or has been added anonymously                                    |
| username       | string |                                                                                            |
| email          | string |                                                                                            |
| password       | string | argon2 hashed password                                                                     |
| avatar         | string | avatar url on our CDN                                                                      |

### Relations
