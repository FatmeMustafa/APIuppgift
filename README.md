# /posts

## GET
### Request
`curl -X GET api.softhouse.rocks/posts`

### Response
`curl -i -X GET api.softhouse.rocks/posts`
`Status code: 200 (OK)`

```
[
  {
    "_id": "5caaef896b334800cbf6634a",
    "userId": 2,
    "id": 15,
    "title": "eveniet quod temporibus",
    "body": "reprehenderit quos placeat\nvelit minima officia dolores impedit repudiandae molestiae nam\nvoluptas recusandae quis delectus\nofficiis harum fugiat vitae",
    "__v": 0
  },
  ```
  
## POST
### Request
```
  curl -i -X POST -H "Content-Type:application/json" api.softhouse.rocks/posts -d'{
  "title": "string",
  "body": "string",
  "userId": number excisting
  }'
```
  
