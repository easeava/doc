# 用户

## 用户管理

获取用户基本信息:

```
$bear->user->get($openID);
```

获取粉丝列表:

```
$bear->user->list($start_index = null);
```

黑名单列表获取:

```text
$bear->user->blacklist(string $begin_openid);
```

拉黑用户:

```text
$bear->user->block($opendList);
```

取消拉黑用户:

```text
$bear->user->unblock($opendList);
```

