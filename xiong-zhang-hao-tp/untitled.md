# 入门

## 熊掌号TP

获取熊掌号tp实例:

```
use EaseBaidu\Factory;

$config = [
    'debug' => 1, // 发布前填写或者修改的环境
    'client_id' => 'xxx',
    'secret' => 'xxx',
    'token' => 'xxx',
    'aes_key' => 'xxx',
    'log' => [
        'name' => 'EaseBearTp',
        'level' => 'debug',
        'file' => __DIR__ . '/logs/bear.log',
    ],
];

$bearTP = Factory::bearTP($config);
```

获取用户授权页 URL:

```text
$bearTP->getPreAuthorizationUrl(string $callbackUrl);
```

根据授权码code，换取授权熊掌号的接口调用凭据:

```text
$bearTP->handleAuthorize(string $authorization_code);
```

获取授权熊掌号信息:

```text
$bear = $bearTP->bear(string $client_id, string $refresh_token);
$bear->getAuthorizer();
```

