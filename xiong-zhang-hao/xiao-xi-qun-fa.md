# 消息群发

## 消息群发

发送消息:

```
$bear->broadcasting->sendMessage(MessageInterface $message);
```

文本消息:

```
$bear->broadcasting->sendText(string $message);
```

语音消息:

```text
$bear->broadcasting->sendVoice(string $mediaID);
```

图片消息:

```text
$bear->broadcasting->sendImage(string $mediaID);
```

