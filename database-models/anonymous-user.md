# Anonymous User

### Description

Users who create a new ticket don't need to register themselves. The Anonymous user belongs to the organisation and can only access public Organisation API endpoints.&#x20;

### Attributes

| Attribute    | Type      | Description                                                                                |
| ------------ | --------- | ------------------------------------------------------------------------------------------ |
| uuid         | uuid4     | User id identifying the user. For temp\_users this will also be their authentication token |
| organisation | ManyToOne | The organisation the anoymous User belongs to                                              |
| username     | string    | Random generated                                                                           |
| email        | string    | optional                                                                                   |

### Relations
