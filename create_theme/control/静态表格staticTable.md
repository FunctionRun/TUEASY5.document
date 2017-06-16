# 静态表格\_staticTable 

---

> ## 开发模式

### 参数配置列表

```
{
	'type': 'Table',
	'width': '100%',
	'height': '100%',
	'color': [
		'#239a8d',
		'#e1e8b0',
		'#24aaca',
		'#b8d4c2',
		'#c5d639',
		'#1e93ab',
		'#ebefe1',
		'#52ab5c',
		'#40a3cf',
		'#9cd0c9',
		'#126da8',
		'#cae2c7'
	],
	'Showheader': {
		'show': true
	},
	'windsNum': {
		'num': 5
	},
	'showtitle': {
		'show': 'true',
		'theadContent': '排名',
		'tbodyPrefix': 'NO.',
		'style': {
			'width': '25%',
			'color': '#999',
			'fontSize': '14px'
		}
	},
	'twoTabelheader': {
		'height': '20%',
		'width': '100%',
		'backgroundColor': 'red',
		'alignItems': 'center',
		'display': 'flex',
		'textAlign': 'center'
	},
	'headerInfo': [
		{
			'PV': 'area',
			'title': '姓名',
			'style': {
				'width': '25%',
				'color': '#239a8d',
				'fontSize': '14px'
			}
		},
		{
			'PV': 'pv',
			'title': '流量',
			'style': {
				'width': '25%',
				'color': '#e1e8b0',
				'fontSize': '14px'
			}
		},
		{
			'PV': 'attribute',
			'title': '用户',
			'style': {
				'width': '25%',
				'color': '#24aaca',
				'fontSize': '14px'
			}
		}
	],
	'twoTabelmian': {
		'height': '80%',
		'width': '100%',
		'backgroundColor': 'yellow',
		'overflowX': 'hidden',
		'overflowY': 'visible',
		'textAlign': 'center'
	},
	'twoTabelchileNode': {
		'display': 'flex',
		'height': '20%',
		'borderBottom': '1px solid red',
		'textOverflow': 'ellipsis',
		'overflow': 'hidden',
		'verticalAlign': 'middle',
		'alignItems': 'center',
		'boxSizing': 'border-box'
	},
	'series': [
		{
			'area': '中国',
			'pv': 688,
			'attribute': 'xxxxxxxxxxxxxxxxxxx'
		},
		{
			'area': '香港',
			'attribute': 'xxxxxxxxxxxxxxxxxxx',
			'pv': 688
		}
	]
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
		<td> type | String </td>
		<td> 控件的类型，默认值，不可修改</td>
		<td>'Table'</td>
	</tr>
	<tr>
		<td> width | String </td>
		<td> 表格的宽度 </td>
		<td> 'px' or '%' </td>
	</tr>
	<tr>
		<td> height | String </td>
		<td> 表格的高度 </td>
		<td> 'px' or '%' </td>
	</tr>
	<tr>
		<td> color | Array </td>
		<td> 表格需要用的颜色样式组 </td>
		<td> <pre>
	[
		'#239a8d',
		'#e1e8b0'
	]
		</pre> </td>
	</tr>
	<tr>
		<td> Showheader.show | Bool </td>
		<td>是否显示表格头部 </td>
		<td> true </td>
	</tr>
	<tr>
		<td> windsNum.num | Number </td>
		<td> 当前表格窗口要显示的表格行数 </td>
		<td> true </td>
	</tr>
	<tr>
		<td> showtitle.show | Bool </td>
		<td>是否显示表格标题 </td>
		<td> true </td>
	</tr>
	<tr>
		<td> showtitle.theadContent | String </td>
		<td> 排序列显示的标题内容 </td>
		<td> 'string' </td>
	</tr>
	<tr>
		<td> showtitle.tbodyPrefix | String </td>
		<td> 排序列显示的前缀内容 </td>
		<td> 'string' </td>
	</tr>
	<tr>
		<td> showtitle.style | Object </td>
		<td> 需要排序列的样式 </td>
		<td> <pre>
	{
		'width': '25%',
		'color': '#999',
		'fontSize': '14px'
	}
		</pre> </td>
	</tr>
	<tr>
		<td> twoTabelheader | Object </td>
		<td> 其他列的样式 </td>
		<td> <pre>
	{
		'height': '20%',
		'width': '100%',
		'backgroundColor': 'red',
		'alignItems': 'center',
		'display': 'flex',
		'textAlign': 'center'
	}
		</pre> </td>
	</tr>
	<tr>
		<td> headerInfo | Array </td>
		<td> 除需要排序列的配置数组 </td>
		<td> </td>
	</tr>
	<tr>
		<td> headerInfo.PV | String </td>
		<td> 当前列配置的唯一id </td>
		<td> id </td>
	</tr>
	<tr>
		<td> headerInfo.title | String </td>
		<td> 当前列标题 </td>
		<td> </td>
	</tr>
	<tr>
		<td> headerInfo.style | Object </td>
		<td> 当前列样式 </td>
		<td><pre>
	{
		'width': '25%',
		'color': '#239a8d',
		'fontSize': '14px'
	}
		</pre></td>
	</tr>
	<tr>
		<td> twoTabelmian | Object </td>
		<td> 除标题行外的内容盒子样式 </td>
		<td><pre>
	{
		'height': '80%',
		'width': '100%',
		'backgroundColor': 'yellow',
		'overflowX': 'hidden',
		'overflowY': 'visible',
		'textAlign': 'center'
	}
		</pre></td>
	</tr>
	<tr>
		<td> twoTabelchileNode | Object </td>
		<td> 除标题行外其他内容行样式 </td>
		<td><pre>
	{
		'display': 'flex',
		'height': '20%',
		'borderBottom': '1px solid red',
		'textOverflow': 'ellipsis',
		'overflow': 'hidden',
		'verticalAlign': 'middle',
		'alignItems': 'center',
		'boxSizing': 'border-box'
	}
		</pre></td>
	</tr>
	<tr>
		<td> series | Array\[Object\] </td>
		<td> 内容数据的配置数组 </td>
		<td><pre>
	[
		{
			'列配置id':'内容'
		}
	]
		</pre></td>
	</tr>
</table>



