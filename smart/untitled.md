# 入门

获取智能小程序实例:

```
use EaseBaidu\Factory;

$config = [
    'app_id' => 'xxx',
    'token' => 'xxx',
    'app_key' => 'xxx',
    'aes_key' => 'xxx',
    'log' => [
        'name' => 'EaseBaidu',
        'level' => 'debug',
        'file' => __DIR__ . '/logs/baidu.log',
    ]
];

$app = Factory::smartProgram($config);
```



