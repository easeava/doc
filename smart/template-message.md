# 消息模板

## 消息模板

获取小程序模板库标题列表:

```
$app->template_message->list($offset, $count);
```

获取模板库某个模板标题下的关键词库:

```
$app->template_message->get($id);
```

组合模板并添加至帐号下的个人模板库:

```text
$app->template_message->add($id, $keyword);
```

获取帐号下已存在的模板列表:

```text
$app->template_message->getTemplates($offset, $count);
```

删除帐号下的某个模板:

```text
$app->template_message->delete($templete_id);
```

