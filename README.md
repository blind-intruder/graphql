# graphql

## Interospection Disabled?

Get all querires
```
{  __type(name: \"Query\") {    name fields{name type{name}}    possibleTypes {      name    }  }}
```

Get all Mutations
```
{  __type(name: \"Mutation\") {    name fields{name type{name}}    possibleTypes {      name    }  }}
```

Single Object
```
{__type (name: \"User\") {name fields{name type{name kind ofType{name kind}}}}}
```
