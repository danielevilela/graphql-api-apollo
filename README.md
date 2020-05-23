# graphql-api-apollo
GraphQL API that connects to two data sources: a REST API , fetching data from SpaceX-API, and a SQLite database.  

PLayground available at: 
https://graphql-api-apollo.herokuapp.com/

## Example
### Query
```
{
  launch(id:5){
    id
    mission{
      name
      missionPatch
    }
    rocket{
      id
      name
      type
    }    
    site
  }
}
```

### Response
```
{
  "data": {
    "launch": {
      "id": "5",
      "mission": {
        "name": "RazakSat",
        "missionPatch": "https://images2.imgbox.com/8d/fc/0qdZMWWx_o.png"
      },
      "rocket": {
        "id": "falcon1",
        "name": "Falcon 1",
        "type": "Merlin C"
      },
      "site": "Kwajalein Atoll"
    }
  }
}
```
