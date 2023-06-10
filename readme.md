$ curl -X POST "localhost:8080/v1/user?name=rk-dev"
{"id":2,"name":"rk-dev"}

$ curl -X PUT "localhost:8080/v1/user/2?name=rk-dev-updated"
{"id":2,"name":"rk-dev-updated"}

$ curl -X GET localhost:8080/v1/user
[{"id":2,"name":"rk-dev-updated"}]

$ curl -X GET localhost:8080/v1/user/2
{"id":2,"name":"rk-dev-updated"}

$ curl -X DELETE localhost:8080/v1/user/2
success
