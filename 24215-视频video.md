# 视频\_Video ![](/assets/Video.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'rtsp': false,
    'playState': 'play',
    'muted': false,
    'videoSrc': '../../../public/videos/testVideo.mp4',
    'videoStyle': {

    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| rtsp | Bool | √ | false |  | 播放的视频是否支持rtsp\(实时流协议\) |
| playState | String | √ | play | pause、play | 初始化时视频的播放状态。pause视频暂停播放，play视频播放 |
| muted | Bool | √ | false |  | 是否播放音频 |
| videoSrc | String | √ |  |  | 视频播放地址 |
| videoStyle | Object |  |  |  | 视频的样式 |

> 注：
>
> * videoStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他视频样式



