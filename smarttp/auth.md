# 代授权

## 代授权实现小程序业务

实例化:

```
use EaseBaidu\Factory;

$config = [
    // ...
];

$smartTP = new Factory::smartTP($config);
```

获取实例:

```
$smart = $smartTP->smart(string $app_id, string $refresh_token);
```



