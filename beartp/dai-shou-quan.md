# 代授权

## 代授权实现熊掌号业务

实例化:

```
use EaseBaidu\Factory;

$config = [
    // ...
];

$bearTP = new Factory::bearTP($config);
```

获取授权方实例:

```
$bear = $bearTP->bear(string $client_id, string $refresh_token);
```



