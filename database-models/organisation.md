# Organisation

### Attributes

| Attribute   | Type   | Description                                            |
| ----------- | ------ | ------------------------------------------------------ |
| name\*      | string | Name identifying the organisation                      |
| slug\*      | string | Organisation slug, only lowercases without underscores |
| logo        | string | logo url on our CDN                                    |
| description | string |                                                        |

### Relations

* ManyToMany: User - Organisation ⇒ Save their role (admin, agent, superadmin, supervisor, owner)
