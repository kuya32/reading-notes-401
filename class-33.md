# Read: 33 - GraphQL @connection

## GraphQL @connection section

- The @connection directive enables you to specify relationships between @model types.
  - Currently, this supports one-to-one, one-to-many, and many-to-one relationships.
  - ```directive @connection(keyName: String, fields: [String!]) on FIELD_DEFINITION```
- Example of all connections
- One to One
![One to One Relationship](img/oneToOneGraph.PNG)

- One to Many
![One to Many Relationship](img/oneToManyGraph.PNG)

- Many to One
![Many to One Relationship](img/manyToOneGraph.PNG)

- Many to Many
![Many to Many Relationship](img/manyToManyGraph.PNG)

[Back to README](README.md)
