# 服务端

## 基本使用

设置消息处理器:

```
$bear->server->push(function ($message) {
    switch ($message['MsgType']) {
        case 'event':
            return '收到事件消息';
            break;
        case 'text':
            return '收到文字消息';
            break;
        default:
            return '收到其它消息';
            break;
    }
    
    // TODO...
})

$response = $bear->server->serve();
$response->send();
```

获取`$message`参数:

```
$message = $server->getMessage();
```

## 注册多个消息处理器

注册多个 handler：

```text
$app->server->push(OtherHandler::class);
$app->server->push(...);
```

