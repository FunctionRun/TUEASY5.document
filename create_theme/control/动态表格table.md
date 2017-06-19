# 动态表格\_Table

---

> ## 开发模式

### 参数配置列表

```
{
	'type': 'Table',
	'width': '100%',
	'height': '100%',
	'animate': {
		'show': 'true',
		'type': 'single',
		'animationTime': 10,
		'stopInterval': 500
	},
	'color': [
		'#239a8d',
		'#e1e8b0'
	],
	'tableRows': {
		'rows': 5
	},
	'theadStyle': {
		'show': true
	},
	'index': {
		'show': true,
		'theadContent': '排名',
		'tbodyPrefix': 'NO.',
		'style': {
			'width': '20%',
			'color': '#999',
			'fontSize': '14px'
		}
	},
	'dataTitle': [
		{
			'PV': 'subType',
			'title': '作物估产',
			'style': {
				'width': '20%',
				'color': '#239a8d',
				'fontSize': '14px'
			}
		},
		{
			'PV': 'type',
			'title': '数字城市',
			'style': {
				'width': '20%',
				'color': '#e1e8b0',
				'fontSize': '14px'
			}
		},
		{
			'PV': 'long',
			'title': '用户',
			'style': {
				'width': '20%',
				'color': '#239a8d',
				'fontSize': '14px'
			}
		},
		{
			'PV': 'lat',
			'title': '用户',
			'style': {
				'width': '20%',
				'fontSize': '14px',
				'color': '#e1e8b0'
			}
		}
	],
	'header': {
		'alignItems': 'center',
		'backgroundColor': '#134458',
		'height': '15%',
		'textOverflow': 'ellipsis',
		'whiteSpace': 'nowrap',
		'overflow': 'hidden',
		'verticalAlign': 'middle',
		'textAlign': 'center',
		'display': 'flex'
	},
	'serieStyle': {
		'width': '100%',
		'overflow': 'hidden',
		'textAlign': 'center'
	},
	'seriesValueStyle': {
		'textOverflow': 'ellipsis',
		'overflow': 'hidden',
		'verticalAlign': 'middle',
		'display': 'flex',
		'alignItems': 'center',
		'backgroundColor': 'rgb(10, 39, 50)',
		'borderBottom': '1px solid #ccc',
		'boxSizing': 'border-box',
		'pointerEvents': 'none',
		'height': '20%'
	},
	'series': [
		{
			'subType': '作物估产',
			'type': '数字城市',
			'long': 105.42964146619371,
			'lat': 34.02673676626235
		},
		{
			'subType': '作物估产',
			'type': '土地覆盖',
			'long': 102.75941818425892,
			'lat': 34.53054408324994
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
		<td> animate.show | Bool </td>
		<td> 动画是否显示</td>
		<td> true </td>
	</tr>
	<tr>
		<td> animate.type | Object </td>
		<td> 动画类型</td>
		<td> single (single,all,none) </td>
	</tr>
	<tr>
		<td> animate.animationTime | Number </td>
		<td> 动画速度</td>
		<td> 10 </td>
	</tr>
	<tr>
		<td> animate.stopInterval | Number </td>
		<td> 动画间隔时间</td>
		<td> 500 </td>
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
		<td> tableRows.rows | Number </td>
		<td> 当前表格窗口要显示的表格行数 </td>
		<td> 5 </td>
	</tr>
	<tr>
		<td> theadStyle.show | Bool </td>
		<td> 是否显示表格标题行 </td>
		<td> true </td>
	</tr>
	<tr>
		<td> index.show | Bool </td>
		<td> 需要排序列配置 </td>
		<td> true </td>
	</tr><tr>
		<td> index.theadContent | String </td>
		<td> 排序列显示的标题内容 </td>
		<td> 'string' </td>
	</tr>
	<tr>
		<td> index.tbodyPrefix | String </td>
		<td> 排序列显示的前缀内容 </td>
		<td> 'string' </td>
	</tr>
	<tr>
		<td> index.style | Object </td>
		<td> 需要排序列的样式 </td>
		<td> <pre>
	{
		'width': '20%',
		'color': '#999',
		'fontSize': '14px'
	}
		</pre> </td>
	</tr>
	<tr>
		<td> dataTitle.PV | String </td>
		<td> 当前列配置的唯一id </td>
		<td> id </td>
	</tr>
	<tr>
		<td> dataTitle.title | String </td>
		<td> 当前列标题 </td>
		<td> </td>
	</tr>
	<tr>
		<td> dataTitle.style | Object </td>
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
		<td> header | Object </td>
		<td> 标题行样式 </td>
		<td><pre>
	{
		'alignItems': 'center',
		'backgroundColor': '#134458',
		'height': '15%',
		'textOverflow': 'ellipsis',
		'whiteSpace': 'nowrap',
		'overflow': 'hidden',
		'verticalAlign': 'middle',
		'textAlign': 'center',
		'display': 'flex'
	}
		</pre></td>
	</tr>
	<tr>
		<td> serieStyle | Object </td>
		<td> 除标题行外的内容盒子样式 </td>
		<td><pre>
	{
		'width': '100%',
		'overflow': 'hidden',
		'textAlign': 'center'
	}
		</pre></td>
	</tr>
	<tr>
		<td> seriesValueStyle | Object </td>
		<td> 除标题行外其他内容行样式 </td>
		<td><pre>
	{
		'textOverflow': 'ellipsis',
		'overflow': 'hidden',
		'verticalAlign': 'middle',
		'display': 'flex',
		'alignItems': 'center',
		'backgroundColor': 'rgb(10, 39, 50)',
		'borderBottom': '1px solid #ccc',
		'boxSizing': 'border-box',
		'pointerEvents': 'none',
		'height': '20%'
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


