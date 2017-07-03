# 时间轴\_TimeLine 

---
![](/assets/Timeline01.png)
![](/assets/Timeline03.png)
![](/assets/Timeline04.png)
![](/assets/Timeline05.png)
![](/assets/Timeline06.png)

> ## 开发模式
![](/assets/Timeline02.png)
### 参数配置列表

```
{
	'type': 'timeLine',
	'selectedType': 'year',
	'selectedValue': {
		'year': [
			2017
		],
		'month': [
			6
		],
		'day': [
			28
		],
		'hour': [
			18
		],
		'season': [
			2
		],
		'tenDays': [
			1
		]
	},
	'autoPlay': {
		'play': false,
		'animationDuration': 2000,
		'animationDelay': 1000,
		'enabledFutureDate': false,
		'disabledStyle': {
			'backgroundColor': 'violet',
			'color': 'gray',
			'cursor': 'not-allowed'
		}
	},
	'choiceModel': 'singleChoice',
	'timeList': [
		{
			'name': '年',
			'value': 'year'
		},
		{
			'name': '季',
			'value': 'season'
		},
		{
			'name': '月',
			'value': 'month'
		},
		{
			'name': '旬',
			'value': 'tenDays'
		},
		{
			'name': '日',
			'value': 'day'
		},
		{
			'name': '时',
			'value': 'hour'
		}
	],
	'dateConfig': [
		{
			'name': 'year',
			'start': 2010,
			'step': 10
		},
		{
			'name': 'season',
			'start': 2,
			'step': 3
		},
		{
			'name': 'month',
			'start': 3,
			'step': 1
		},
		{
			'name': 'tenDays',
			'start': 1,
			'step': 5
		},
		{
			'name': 'day',
			'start': 2,
			'step': 1
		},
		{
			'name': 'hour',
			'start': 6,
			'step': 1
		}
	],
	'timeLineStyle': {
		'borderTop': '2px solid #b2bac3',
		'borderBottom': '2px solid #b2bac3'
	},
	'timeHeader': {
		'itemStyle': {
			'backgroundColor': '#eff1f3',
			'marginRight': '5px',
			'width': '300px'
		},
		'labelStyle': {
			'color': '#667688',
			'fontSize': '20px'
		},
		'iconStyle': {
			'color': '#ffa84e',
			'fontSize': '20px',
			'padding': '5px'
		}
	},
	'timeBody': {
		'normal': {
			'color': '#999999',
			'width': 'calc(100% - 300px - 80px)'
		},
		'emphasis': {

		}
	},
	'timeFooter': {
		'normal': {
			'color': '#84b0ed',
			'width': '80px',
			'backgroundColor': '#eff1f3'
		},
		'emphasis': {
			'color': '#ffa84e',
			'width': '80px',
			'backgroundColor': '#f4e7d9'
		}
	},
	'footerList': {
		'normal': {
			'color': '#84b0ed',
			'width': '80px',
			'height': '50px',
			'lineHeight': '50px',
			'backgroundColor': '#eff1f3'
		},
		'emphasis': {
			'color': '#ffa84e',
			'width': '80px',
			'height': '50px',
			'lineHeight': '50px',
			'backgroundColor': '#f4e7d9'
		}
	},
	'timeZoom': {
		'normal': {
			'backgroundColor': 'rgba(179, 212, 252, 1)'
		},
		'emphasis': {
			'backgroundColor': 'rgba(255, 168, 78, 1)'
		}
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
		<td> selectedType | String </td>
		<td>当前选中的时间类型</td>
		<td>year</td>
	</tr>
	<tr>
		<td> selectedValue | Object </td>
		<td>选中的值域</td>
		<td><pre>
			{
		        'year': [
		            2017
		        ],
		        'month': [
		            6
		        ],
		        'day': [
		            28
		        ],
		        'hour': [
		            18
		        ],
		        'season': [
		            2
		        ],
		        'tenDays': [
		            1
		        ]
	        }
		</pre></td>
	</tr>
	<tr>
		<td> autoPlay | Object </td>
		<td>是否自动执行时间轴动画</td>
		<td><pre>
			{
		        'play': false,
		        'animationDuration': 2000,
		        'animationDelay': 1000,
		        'enabledFutureDate': false,
		        'disabledStyle': {
		            'backgroundColor': 'violet',
		            'color': 'gray',
		            'cursor': 'not-allowed'
		        }
		    }
		</pre></td>
	</tr>
	<tr>
		<td> choiceModel | String </td>
		<td> 时间轴选择模型 </td>
		<td> singleChoice </td>
	</tr>
	<tr>
		<td> timeList | Object </td>
		<td> 时间列表 </td>
		<td><pre>
			[
		        {
		            'name': '年',
		            'value': 'year'
		        },
		        {
		            'name': '季',
		            'value': 'season'
		        },
		        {
		            'name': '月',
		            'value': 'month'
		        },
		        {
		            'name': '旬',
		            'value': 'tenDays'
		        },
		        {
		            'name': '日',
		            'value': 'day'
		        },
		        {
		            'name': '时',
		            'value': 'hour'
		        }
		    ]
		</pre></td>
	</tr>
	<tr>
		<td> dateConfig | Object </td>
		<td> 日期配置 </td>
		<td><pre>
			[
        {
            'name': 'year',
            'start': 2010,
            'step': 10
        },
        {
            'name': 'season',
            'start': 2,
            'step': 3
        },
        {
            'name': 'month',
            'start': 3,
            'step': 1
        },
        {
            'name': 'tenDays',
            'start': 1,
            'step': 5
        },
        {
            'name': 'day',
            'start': 2,
            'step': 1
        },
        {
            'name': 'hour',
            'start': 6,
            'step': 1
        }
    ]
		</pre></td>
	</tr>
	<tr>
		<td> timeLineStyle | Object </td>
		<td> 时间轴边框样式 </td>
		<td><pre>
			{
		        'borderTop': '2px solid #b2bac3',
		        'borderBottom': '2px solid #b2bac3'
		    }
		</pre></td>
	</tr>
	<tr>
		<td> timeHeader | Object </td>
		<td> 时间轴头部所选时间样式 </td>
		<td><pre>
			{
				'itemStyle': {
					'backgroundColor': '#f00',
					'marginRight': '5000px',
					'width': '300px'
				},
				'labelStyle': {
					'color': '#667688',
					'fontSize': '20px'
				},
				'iconStyle': {
					'color': '#ffa84e',
					'fontSize': '20px',
					'padding': '5px'
				}
			}
		</pre></td>
	</tr>
	<tr>
		<td> timeBody | Object </td>
		<td> 时间轴内容样式 </td>
		<td><pre>
			{
				'normal': {
					'color': '#999999',
					'width': 'calc(100% - 300px - 80px)'
				},
				'emphasis': {

				}
			}
		</pre></td>
	</tr>
	<tr>
		<td> timeFooter | Object </td>
		<td> 末尾处所选择时间类型值的样式 </td>
		<td><pre>
			{
				'normal': {
					'color': '#84b0ed',
					'width': '80px',
					'backgroundColor': '#eff1f3'
				},
				'emphasis': {
					'color': '#ffa84e',
					'width': '80px',
					'backgroundColor': '#f4e7d9'
				}
			}
		</pre></td>
	</tr>
	<tr>
		<td> footerList | Object </td>
		<td> 时间轴两边所选时间值域的样式 </td>
		<td><pre>
			{
				'normal': {
					'color': '#84b0ed',
					'width': '80px',
					'height': '50px',
					'lineHeight': '50px',
					'backgroundColor': '#eff1f3'
				},
				'emphasis': {
					'color': '#ffa84e',
					'width': '80px',
					'height': '50px',
					'lineHeight': '50px',
					'backgroundColor': '#f4e7d9'
				}
			}
		</pre></td>
	</tr>
	<tr>
		<td> timeZoom | Object </td>
		<td> 时间缩放区域样式 </td>
		<td><pre>
			{
				'normal': {
					'backgroundColor': 'rgba(179, 212, 252, 1)'
				},
				'emphasis': {
					'backgroundColor': 'rgba(255, 168, 78, 1)'
				}
			}
		</pre></td>
	</tr>
</table>


