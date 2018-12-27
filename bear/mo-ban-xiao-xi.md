# 模板消息

## 模板消息

获取已添加的模板列表:

```
$bear->template_message->getPrivateTemplates();
```

获取系统模板列表:

```
$bear->template_message->getSysTemplates(string $kw, int $pn = 1, int $ps = 10);
```

添加模板:

```text
$bear->template_message->addTemplate(string $id);
```

删除模板

```text
$bear->template_message->deletePrivateTemplate(string $template_id);
```

发送模板消息:

```text
$bear->template_message->send(array $message);
```

