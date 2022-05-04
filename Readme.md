To add new mock to smoker:
```
  curl --request POST \
    --url http://localhost:8081/mocks \
    --header 'Content-type: application/json' \
    --data '[
    {
      "request": {
        "method": "GET",
        "path": "/maps/api/place/textsearch/json"
      },
      "response": {
        "status": 200,
        "headers": {
          "Content-Type": "application/json"
        },
        "body": "{\n  \"city\": \"Kyiv\"\n}\n"
      }
    }
  ]'
```
