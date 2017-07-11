# 外接\_iframe 

---

> ## 开发模式
![](/assets/Iframe.png)
### 参数配置列表

```
{
    'src': 'http://www.hiynn.com',
	'frameBorder': 1,
	'style': {
		'borderWidth': 10,
		'borderColor': '#333'
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
		<td> src | String </td>
		<td>iframe的地址路径</td>
		<td> 'http://www.hiynn.com' </td>
	</tr>
	<tr>
		<td> frameBorder | Number </td>
		<td>iframe外边线的宽度</td>
		<td> 1 </td>
	</tr>
	<tr>
		<td>style | Object </td>
		<td>iframe的样式</td>
		<td><pre>
	{
		'borderWidth': 10,
		'borderColor': '#333'
	}
		</pre></td>
	</tr>
</table>

