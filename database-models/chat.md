# Chat

### Attributes

| Attribute       | Type      | Description                                |
| --------------- | --------- | ------------------------------------------ |
| chat\_id        | int       | logo url on our CDN                        |
| created\_by     | ManyToOne | User who created the ticket                |
| assigned\_to    | ManyToOne | Agent who is assigned to this ticket       |
| status          | string    | Status according to definition             |
| last\_updated   | datetime  |                                            |
| status\_payload | string    | payload according to the status definition |

### Relations
