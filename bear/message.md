# 消息

## 消息

文本消息:

```
use EaseBaidu\Kernel\Message\Text;

$text = new Text('您好！easebaidu.');

// or
$text = new Text();
$text->content = '您好！easebaidu.';

// or
$text = new Text();
$text->setAttribute('content', '您好！easebaidu');
```

图片消息:

```
use EaseBaidu\Kernel\Message\Image;

$image = new Image($mediaID);
```

语音消息:

```text
use EaseBaidu\Kernel\Message\Voice;

$image = new Voice($mediaID);
```

