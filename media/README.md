# 多媒体开发

由于性能和硬件关联问题，音视频开发绝大多数都是使用 C/C++ 开发的。

音视频主要设计到几个方面：

1. 音视频同步，编解码：FFmpeg（软解码）， H264 编码原理。
2. MediaCodec 硬件码
3. Rtmp 协议实现直播拉流（看直播）
4. 硬编码下实现直播推流
5. 音视频编辑技术
6. 特效制作： OpenGL ES
7. WebRTC 实现 PTP 语音通话
8. 多人视频会议（降噪，回声消除）。

```
音/视频录制 --> 编码(封装) --> 编辑 -------┐
                                   传输(推送/拉取)
播放       <-- 解码      <-- 编辑 <------┘
```

- [Ffmpeg](ffmpeg/README.md)