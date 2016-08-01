# rest-flask
Simple REST API SERVER in Flask. This repository created for learning purposes.

# Description
This is 'ToDo' management REEST Server.

# APIs

**Base URL**

```
http://localhost:5000/todo/api/tasks
```

Need basic Authorize, specify the following options.

```
-u user:password
```

If you do not change the script looks like this.

```
-u kamiya:python
```

## GET

##### Get All Tasks

```
curl -i http://localhost:5000/todo/api/tasks
```

##### Get Specified Task

```
curl -i http://localhost:5000/todo/api/task/1
```

## POST

```
curl -i -H "Content-Type: application/json" -X POST -d '{"title":"本を読む"}' http://localhost:5000/todo/api/tasks
```

## PUT

```
curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/tasks/1
```

## DELETE

```
curl -X DELETE http://localhost:5000/todo/api/1
```

# NOTE

You if you are using windows or Or if you are not familiar with operations at a black screen
It is recommended to use this tool.

[postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop)
