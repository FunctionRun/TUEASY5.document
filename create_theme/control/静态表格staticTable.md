# 静态表格\_staticTable 

---

![](/assets/StaticTable01.png)
![](/assets/StaticTable02.png)

## 开发模式
![](/assets/StaticTable03.png)
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
    'theadStyle': {
        'show': true
    },
    'tableRows': {
        'num': 5
    },
    'index': {
        'show': true,
        'theadContent': '排名',
        'tbodyPrefix': 'NO.',
        'style': {
            'width': '25%',
            'color': '#999',
            'fontSize': '14px'
        }
    },
    'header': {
        'height': '20%',
        'width': '100%',
        'backgroundColor': 'red',
        'alignItems': 'center',
        'display': 'flex',
        'textAlign': 'center'
    },
    'dataTitle': [
        {
            'PV': 'area',
            'title': '姓名',
            'style': {
                'width': '25%',
                'color': '#999',
                'fontSize': '14px'
            }
        },
        {
            'PV': 'pv',
            'title': '流量',
            'style': {
                'width': '25%',
                'color': '#999',
                'fontSize': '14px'
            }
        },
        {
            'PV': 'attribute',
            'title': '用户',
            'style': {
                'width': '25%',
                'color': '#999',
                'fontSize': '14px'
            }
        }
    ],
    'herderItemStyle': {
        'normalStyle': {
            'fontSize': '14px',
            'backgroundColor': 'yellow'
        },
        'emphasisStyle': {
            'fontSize': '18px',
            'backgroundColor': 'red'
        }
    },
    'serieStyle': {
        'height': '80%',
        'width': '100%',
        'backgroundColor': 'yellow',
        'overflowX': 'hidden',
        'overflowY': 'visible',
        'textAlign': 'center'
    },
    'seriesValueStyle': {
        'display': 'flex',
        'height': '20%',
        'borderBottom': '1px solid red',
        'textOverflow': 'ellipsis',
        'overflow': 'hidden',
        'verticalAlign': 'middle',
        'alignItems': 'center',
        'boxSizing': 'border-box'
    },
    'itemStyle': {
        'normalStyle': {
            'fontSize': '14px',
            'backgroundColor': 'yellow'
        },
        'emphasisStyle': {
            'fontSize': '18px',
            'backgroundColor': 'red'
        }
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
        },
        {
            'area': '中国',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx',
            'data': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '香港',
            'pv': 688,
            'attribute': 'attributexxxxxxxxxxxxxxxxxxx',
            'data': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '俄罗斯',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '德国',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '吉尔吉斯斯坦',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '英国',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '日本',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '南非',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '巴西',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '印度',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '新加坡',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '加拿大',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '澳大利亚',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '阿根廷',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '西班牙',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '墨尔本',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '乌卡卡',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '蓝卡卡',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '自卡卡',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
        },
        {
            'area': '你卡看',
            'pv': 688,
            'attribute': 'xxxxxxxxxxxxxxxxxxx'
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



