# 网页授权

发起授权:

```
$response = $bear->oauth->redirect();
$response->send();
```

获取已授权用户:

```text
$user = $bear->oauth->user();
```



