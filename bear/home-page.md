# 主页管理

## 主页管理

自定义tab创建:

```
$bear->home_page->create(array $tabs);
```

自定义tab修改:

```
$bear->home_page->update(array $tabs);
```

自定义tab删除:

```text
$bear->home_page->delete();
```

获取自定义tab下详细内容:

```text
$bear->home_page->tabinfo(int $page = 1, int $pagesize = 0);
```

编辑自定义tab下产品／精选／专栏内容:

```text
$bear->home_page->updateTabinfo(array $tabs);
```

新建单个自定义tab下产品／精选／专栏内容:

```text
$bear->home_page->createArticle(array $article);
```

修改单个自定义tab下产品／精选／专栏内容:

```text
$bear->home_page->updateArticle(int $itemID, array $article);
```

批量删除自定义tab下产品／精选／专栏内容:

```text
$bear->home_page->deleteArticles(array $itemids);
```

物料上传:

```text
$bear->home_page->uploadStuff(string $path, int $type); // 文件方式上传物料
$bear->home_page->uploadMaterial(string $file, int $type); // base64图片流方式上传图片类型物料
```

运营位状态管理:

```text
$bear->home_page->operationStatus(); // 获取运营位状态
$bear->home_page->setoperationStatus(int $status); // 删除运营位
```

运营位信息管理:

```text
$bear->home_page->openoperation(); // 获取运营位信息
$bear->home_page->addOpenoperation(string $title, string $url, string $tag); // 添加运营位信息
$bear->home_page->updateOpenoperation(int $id, array $openoperation); // 更新运营位信息
```

背景图位信息管理:

```text
$bear->home_page->background(); // 获取背景图位信息
$bear->home_page->deleteBackground(); // 删除号首页背景图位信息
$bear->home_page->publishBackground(int $stuff_id);  // 发布背景图位信息
```



