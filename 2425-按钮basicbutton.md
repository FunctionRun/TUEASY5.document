# 按钮\_basicButton ![](/assets/basicButton.png)

---

> ## 编辑模式

用户可以通过下方的用户编辑模式面板实现对按钮样式的快速编辑。![](/assets/buttonUser.jpg)

> ## 开发模式

### 参数配置列表

```
{
	'type': 'TheButton',
	'normal': {
		'backgroundColor': '#31b16c',
		'fontSize': '20',
		'borderRadius': 5,
		'borderColor': '#31b16c',
		'borderWidth': 1,
		'borderStyle': 'solid',
		'color': '#fff',
		'lineHeight': '47px',
		'textAlign': 'center',
		'cursor': 'pointer',
		'opacity': 0.6
	},
	'mouse': {
		'backgroundColor': '#31b16c',
		'borderRadius': 5,
		'fontSize': '20',
		'borderColor': '#31b16c',
		'borderWidth': 1,
		'borderStyle': 'solid',
		'color': '#fff',
		'lineHeight': '47px',
		'textAlign': 'center',
		'cursor': 'pointer',
		'opacity': 0.8
	},
	'emphasis': {
		'backgroundColor': '#31b16c',
		'borderRadius': 5,
		'fontSize': '20',
		'lineHeight': '47px',
		'color': '#fff',
		'textAlign': 'center',
		'borderColor': '#31b16c',
		'borderWidth': 1,
		'borderStyle': 'solid',
		'opacity': 0.7
	},
	'selected': false,
	'text': '确 认'
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
	<td>type | String</td>
	<td>控件类型——Button按钮，不可修改</td>
	<td>Button</td>
</tr>
<tr>
	<td>normal | Object</td>
	<td>按钮<b>未选中</b>状态的样式</td>
	<td><pre> {
	//背景颜色，支持CSS3中颜色的参数值
	'backgroundColor': '#31b16c',
	//文本大小，支持CSS3中font-size的参数值
	'fontSize': '20px',
	//边框圆角角度，支持CSS3中border-radius的参数值
	'borderRadius': '5px'
	//边框颜色，支持CSS3中border-color的参数值
	'borderColor': '#31b16c',
	//边框宽度，支持CSS3中border-width的参数值
	'borderWidth': 1px,
	//边框样式，支持CSS3中border-style的参数值
	'borderStyle': 'solid',
	//文本颜色，支持CSS3中颜色的参数值
	'color': '#fff'
	//文本行间距，支持CSS3中line-height的参数值
	'lineHeight': '47px',
	//文本水平对齐方式，支持CSS3中text-align的参数值
	'textAlign': 'center',
	//鼠标样式，支持CSS3中cursor的参数值
	'cursor': 'pointer',
	//透明度，支持CSS3中opacity的参数值
	'opacity': 0.6
  }</pre></td>
</tr>
<tr>
	<td>mouse | Object</td>
	<td>按钮<b>鼠标悬浮</b>状态的样式</td>
	<td><pre> {
	'backgroundColor': '#31b16c',
	'fontSize': '20px',
	'borderRadius': '5px'
	'borderColor': '#31b16c',
	'borderWidth': 1px,
	'borderStyle': 'solid',
	'color': '#fff'
	'lineHeight': '47px',
	'textAlign': 'center',
	'cursor': 'pointer',
	'opacity': 0.8
  }</pre></td>
</tr>
<tr>
	<td>emphasis | Object</td>
	<td>按钮<b>选中</b>状态的样式</td>
	<td><pre> {
	'backgroundColor': '#31b16c',
	'fontSize': '20px',
	'borderRadius': '5px'
	'borderColor': '#31b16c',
	'borderWidth': 1px,
	'borderStyle': 'solid',
	'color': '#fff'
	'lineHeight': '47px',
	'textAlign': 'center',
	'cursor': 'pointer',
	'opacity': 0.7
  }</pre></td>
</tr>
<tr>
	<td>selected | Bool</td>
	<td>是否为选中状态</td>
	<td></td>
</tr>
<tr>
	<td>text | String</td>
	<td>按钮的文本内容</td>
	<td></td>
</tr>
</table>

> 注：
>
> * normal、mouse、emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他按钮样式



