# rest-flask
Simple REST API SERVER in Flask. This repository created for learning purposes.

Flaskで作成されたなREST APIサーバです。このリポジトリは勉強のために作成しました。

# Description
This is 'ToDo' management REEST Server.

これは'ToDo'を管理するためのRESTサーバです。

# APIs

**Base URL**

```
http://localhost:5000/todo/api/tasks
```

Need basic Authorize, specify the following options.

Basic認証が必要です。以下のオプションを指定してください。

```
-u user:password
```

If you do not change the script looks like this.

もしスクリプトを変更していない場合は、以下のようになります。
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

もしあなたがWindowsマシンを使っていたり、黒い画面に慣れていない場合は、以下のアプリケーションを使うと幸せになれます。

It is recommended to use this tool.
[postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop)


