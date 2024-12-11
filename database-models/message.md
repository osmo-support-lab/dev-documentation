# Message

### Attributes

| Attribute           | Type      | Description                                                                    |
| ------------------- | --------- | ------------------------------------------------------------------------------ |
| chat                | ManyToOne | Chat the message belongs to                                                    |
| created\_by         | ManyToOne | User who created the message                                                   |
| created\_on         | datetime  | Creation timestamp                                                             |
| is\_chat\_agent     | boolean   | Whether the message is sent by a chat agent                                    |
| is\_system\_message | boolean   | Whether the message is a system message (e.g. status change, assigned to, ...) |
| is\_internal\_note  | boolean   | Whether the message is an internal note (only visible to admins)               |
| user\_status        | string    | User status according to definition                                            |
| agent\_status       | string    | Agent status according to definition                                           |

### Relations
