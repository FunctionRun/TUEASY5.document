# 视频\_Video ![](/assets/Video.png)

---
![](/assets/Video01.png)
## 开发模式
![](/assets/Video02.png)
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

<table border="1">
	<tr>
		<th width="15%">配置项</th>
		<th width="30%">功能/描述</th>
		<th>可选参数</th>
	</tr>
	<tr>
		<td> rtsp | Bool </td>
		<td>播放的视频是否支持rtsp\(实时流协议\)</td>
		<td>false</td>
	</tr>
	<tr>
		<td> playState | String </td>
		<td>初始化时视频的播放状态。pause视频暂停播放，play视频播放</td>
		<td>play (pause、play)</td>
	</tr>
	<tr>
		<td> muted | Bool </td>
		<td>是否播放音频</td>
		<td>false</td>
	</tr>
	<tr>
		<td> videoSrc | String </td>
		<td>视频播放地址</td>
		<td> '../../../public/videos/testVideo.mp4' </td>
	</tr>
	<tr>
		<td> videoStyle | Object </td>
		<td>视频的样式 </td>
		<td><pre>
			{
				'width': '20px'
			}
		</pre></td>
	</tr>
</table>

> 注：
>
> * videoStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他视频样式



