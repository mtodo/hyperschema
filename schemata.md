## <a name="resource-signup"></a>Sign up

Resource representing new user to be created

### Sign up 

Create new user

```
POST /signup
```

#### Required Parameters

| Name | Type | Description | Example |
| ------- | ------- | ------- | ------- |
| **email** | *email* | New user's email | `"username@example.com"` |
| **password** | *string* | New user's password | `"example"` |
| **confirm** | *string* | New user's password confirmation. Should match `password` field | `"example"` |



#### Curl Example

```bash
$ curl -n -X POST http://mtodoapp.com/api/signup \
  -H "Content-Type: application/json" \
 \
  -d '{
  "email": "username@example.com",
  "password": "example",
  "confirm": "example"
}'
```


#### Response Example

```
HTTP/1.1 201 Created
```

```json
{
}
```


