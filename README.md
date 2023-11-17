# Haikyuu-Characters-API

### Example Usage

``` 
curl http://localhost:3000/api/posts
```

Response

```json
{
    "status": true,
    "message": "List Data Posts",
    "data": [
        {
            "id": 16,
            "name": "Taketora Yamamoto",
            "position": "Wing Spiker / Outside Hitter / Ace",
            "status": "Active",
            "team_name": "Nekoma"
        },
        {
            "id": 15,
            "name": "Morisuke Yaku",
            "position": "Libero",
            "status": "Active",
            "team_name": "Nekoma"
        },
```

You can request a specific character by passing the GET parameter `id` if you know its ID/order.

```bash
curl http://localhost:3000/api/posts/10
```

Response

```json
{
    "status": true,
    "message": "Detail Data Post",
    "data": {
        "id": 10,
        "name": "Shōyō Hinata",
        "position": "Middle Blocker / Decoy",
        "status": "Active",
        "team_name": "Karasuno"
    }
}
```
