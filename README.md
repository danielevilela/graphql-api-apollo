<h1 align="center">
  🚀Space-x GraphQL Api
</h1>

<h1>
  <img src="public/graphql-api.gif">
</h1>

## ✔ About
This project was built via Apollo Documentation as part of my studies. It' a GraphQL API that connects to two data sources: a REST API , fetching data from [SpaceX-API](https://api.spacexdata.com/v2/), and a SQLite database.

🟢 [Playground](https://graphql-api-apollo.herokuapp.com/)


---
## ⚙ Tech
- JavaScript
- Node.js
- GraphQL
- Apollo
- SQLite

---

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
