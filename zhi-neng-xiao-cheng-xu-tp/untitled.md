# 入门

## 智能小程序TP

获取小程序tp实例:

```
use EaseBaidu\Factory;

$config = [
    'client_id' => 'xxx',
    'token' => 'xxx',
    'app_key' => 'xxx',
    'aes_key' => 'xxx',
    'log' => [
        'name' => 'EaseBaidu',
        'level' => 'debug',
        'file' => __DIR__ . '/logs/smarttp.log',
    ]
];

$smartTP = Factory::smartProgram($config);
```

获取用户授权页 URL:

```text
$smartTP->getPreAuthorizationUrl(string $callbackUrl);
```

使用授权码换小程序的接口调用凭据和授权信息:

```text
$smartTP->handleAuthorize(string $code = null);
```

获取小程序基础信息:

```text
$smartTP->getAuthorizer(string $access_token);
```

