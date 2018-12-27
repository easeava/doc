# 包管理

## 小程序包管理

为授权的小程序帐号上传小程序代码:

```
$smart->upload(int $template_id, int $ext_json, string $user_version, string $user_desc);
```

为授权的小程序提交审核:

```
$smart->submitAudit(string $content, string $package_id, string $remark);
```

发布已通过审核的小程序:

```text
$smart->release(string $package_id);
```

小程序版本回退:

```text
$smart->rollback(string $package_id);
```

小程序审核撤回:

```text
$smart->withdraw(string $package_id);
```

获取授权小程序预览包详情:

```text
$smart->getTrial();
```

获取小程序包列表:

```text
$smart->list();
```

获取授权小程序包详情:

```text
$smart->getDetail(int $type = null, int $package_id = null);
```

