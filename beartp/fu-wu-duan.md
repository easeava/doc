# 服务端

## 服务端

第三方平台推送事件:

```
$server = $bearTP->server;

return $server->serve();
```

{% hint style="info" %}
 SDK 默认处理`verify_ticket`事件, 并缓存`Ticket.`
{% endhint %}

自定义消息处理器:

```
$server->push(function ($message) {
    // ...
}, 'authorized');

// TODO...
```



