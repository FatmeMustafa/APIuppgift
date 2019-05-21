# /posts

## GET
### Request
`curl -i -X GET api.softhouse.rocks/posts`
### Response
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
  "title": "Hi, World",
  "body": "Fresh as morning dew",
  "userId": "1"
  }'
```
### Response
`Status code: 201 (Created)`


# /posts/{postId}

## GET
### Request
`curl -i -X GET api.softhouse.rocks/posts/3`

### Response
`Status code: 200 (OK) (Even when not found)`
```
 {
  "_id": "5caaef896b334800cbf6633e",
  "userId": 1,
  "id": 3,
  "title": "some other name",
  "body": "et iusto sed quo iure\nvoluptatem occaecati omnis eligendi aut ad\nvoluptatem doloribus vel accusantium quis pariatur\nmolestiae porro eius odio et labore et velit aut",
  "__v": 0
}
