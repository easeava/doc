# 用户标签

## 用户标签

创建标签:

```
$bear->user_tag->create(string $name);
```

获取熊掌号已创建的标签:

```
$bear->user_tag->list();
```

编辑标签:

```text
$bear->user_tag->update(int $tagID, string $name);
```

删除标签:

```text
$bear->user_tag->update(int $tagID);
```

获取标签下粉丝列表:

```text
$bear->user_tag->usersOfTag(int $tagID);
```

批量为用户打标签:

```text
$bear->user_tag->tagUsers(array $openids, int $tagID);
```

批量为用户取消标签:

```text
$bear->user_tag->untagUsers(array $openids, int $tagID);
```

获取用户身上的标签列表:

```text
$bear->user_tag->userTags(int $openid);
```

