# Relations

## ManyToMany

### User - Organisation

|              |           |                                       |
| ------------ | --------- | ------------------------------------- |
| user         | ManyToOne |                                       |
| organisation | ManyToOne |                                       |
| role         | string    | Contains the role (admin, agent, ...) |
