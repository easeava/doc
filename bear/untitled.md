# 入门

获取熊掌号实例:

```
use EaseBaidu\Factory;

$config = [
    'app_id' => 'xxx',
    'client_id' => 'xxx',
    'secret' => 'xxx',
    'token' => 'xxx',
    'aes_key' => 'xxx',
    'log' => [
        'name' => 'EaseBaidu',
        'level' => 'debug',
        'file' => __DIR__ . '/logs/bear.log',
    ]
];

$bear = Factory::bear($config);
```



