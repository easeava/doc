# 基础信息

## 基础信息设置

获取小程序类目:

```text
$smart->$smart->getAllCategories();
```

修改小程序类目:

```text
$smart->updateCategory(array $category);
```

修改小程序icon:

```text
$smart->updateIcon(string $image_url);
```

修改功能介绍:

```text
$smart->updateSignature(string $signature);
```

暂停服务:

```text
$smart->pause();
```

开启服务:

```text
$smart->resume();
```

获取二维码:

```text
$smart->qrcode(string $path = null, string $package_id = null, int $width = 200);
```

小程序名称设置及改名:

```text
$smart->setNickname(string $nick_name);
```

设置最低基础库版本:

```text
$smart->setSupportVersion(string $version);
```

查询当前设置的最低基础库版本及各版本列表:

```text
$smart->getSupportVersion();
```

