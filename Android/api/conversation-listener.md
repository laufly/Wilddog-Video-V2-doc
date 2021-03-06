title: Conversation.Listener
---

视频通话状态回调,当视频通话呼叫状态改变和参与者状态改变时会触发回调方法通知使用者视频通话的状态。

## 方法

### onResponse(CallStatus)

**定义**   

```java
onResponse(CallStatus status)
```

**说明**

视频通话中呼叫状态变更的回调。

**参数**

| 参数名 | 描述 |
|---|---|
|status|[CallStatus](/video/Android/api/call-status.html),连接建立成功后创建的视频通话对象|

</br>

---

### onStreamReceived(RemoteStream);

**定义**   

```java
void onStreamReceived(RemoteStream stream);
```

**说明**

成功接收远端用户发送的媒体流后触发,`Conversation.Listener` 对象通过该方法通知用户收到远端发布的音视频流

**参数**

| 参数名 | 描述 |
|---|---|
|stream|[RemoteStream](/video/Android/api/remote-stream.html),远端参与者发送的媒体流.|

</br>

---

### onError(WilddogVideoError);

**定义**   

```java
void onError(WilddogVideoError error);
```

**说明**

视频通话过程中产生的错误,由此接口回调。

**参数**

| 参数名 | 描述 |
|---|---|
|error|[WilddogVideoError](/video/Android/api/wilddog-video-error.html),视频通话过程中的错误信息|

</br>

---

### onClosed();

**定义**   

```java
onClosed();
```

**说明**

通话结束触发的回调。

</br>

---
