# Managing users via REST API

Develop a REST API microservice for managing users.

Users should be HTTP resources that follow the REST semantics:
- `GET /user/` should list all users in the system
- `GET /user/{id}` should present the user with given id
- `GET /user/?{key}={value}` whould list all users with property being equal value
- `POST /user/` should store new resource
- `PUT /user/{id}` should update a resource
- `DELETE /user/{id}` should remove a resource

Development standard requirements:
- use the respective HTTP Status Codes and other headers where needed
- do not store users in database - keep them in memory for simplicity
- properties of a user resource are up to you

Bonus points for:
- implementing authentication mechanism of any kind for non-GET calls (JWT counts double)
