# 素材管理

## 素材管理

新增图文:

```
$bear->material->uploadArticle($articles);
```

上传图文消息内的图片获取URL:

```
$bear->material->uploadArticleImage(string $path);
```

上传图片:

```text
$bear->material->uploadImage(string $path);
```

上传语音:

```text
$bear->material->uploadVoice(string $path);
```

获取素材:

```text
$bear->material->get(string $mediaID);
```

删除素材:

```text
$bear->material->delete(string $mediaID);
```

修改素材:

```text
$bear->material->updateMaterial(string $mediaID, $article, int $index = 0);
```

获取素材总数:

```text
$bear->material->stats();
```

获取素材列表:

```text
$bear->material->list(string $type, int $offset = 0, int $count = 20);
```



