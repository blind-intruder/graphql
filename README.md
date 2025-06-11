# graphql

## Interospection Disabled?

Get all querires
```
{  __type(name: \"Query\") {    name fields{name type {          name          kind        } }    possibleTypes {      name  fields {        name        type {          name          kind        }      }  }  }}
```

Get all Mutations
```
{  __type(name: \"Mutation\") {    name fields{name type {          name          kind        } }    possibleTypes {      name  fields {        name        type {          name          kind        }      }  }  }}
```

Single Object
```
{__type (name: \"User\") {name fields{name type{name kind ofType{name kind}}}}}
```


Type System Summary

**Category**    |	**Keyword**     |	**Example**
| --------      | -------         | -------
Root Operation  |	type	          | Query, Mutation, Subscription
Object	        | type	          | User, Post
Scalar	        | scalar	        | DateTime, JSON
Enum	          | enum	          | UserStatus
Interface	      | interface	      | Node
Union	          | union	          | SearchResult
Input Object    | input	          | UserInput
List/Non-Null	  | [] and !	      | [String!]!
Introspection	  | Auto-generated	| __Type, __Field
