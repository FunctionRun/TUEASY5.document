# 柱状图/条形图\_visual\_tickBar ![](/assets/text.png)

---

> ## 开发模式

### 参数配置列表

```
{
	'color': [
		'#e38d5d',
		'#6fc6c4',
		'#f0a367',
		'#73e0e5',
		'#0b619a',
		'#e37c97',
		'#f2ecc2',
		'#c42f2e',
		'#f7d733',
		'#667aad',
		'#db781f',
		'#3cadce'
	],
	'grid': [
		{
			'top': 10,
			'right': 50,
			'bottom': 20,
			'left': 50,
			'radius': 10,
			'bgStyle': {
				'normal': {
					'fill': 'rgba(0,0,0,0)'
				},
				'emphasis': {
					'fill': 'rgba(0,0,0,0)'
				}
			}
		}
	],
	'tooltip': {
		'show': true,
		'style': {
			'border-color': '#cc0',
			'border-radius': '5',
			'border-width': '2',
			'border-style': 'solid',
			'width': '100',
			'height': '60',
			'text-align': 'center',
			'line-height': '60',
			'pointer-events': 'none',
			'background-color': 'rgba(255, 255, 255, 0.7)'
		},
		'formatter': function formatter(param) {

	        return param.dataIndex + ': ' + param.value;
	    },
		'position': function position() {

	        return [20, 10];
	    }
	},
	'xAxis': [
		{
			'type': 'linear',
			'inverse': false,
			'axisLine': {
				'show': false,
				'lineStyle': {
					'fill': 'none',
					'stroke': 'yellow',
					'stroke-width': '2',
					'shape-rendering': 'crispEdges'
				}
			},
			'axisLabel': {
				'show': false,
				'interval': 'auto',
				'inside': false,
				'rotate': 0,
				'margin': 8,
				'formatter': null,
				'textStyle': {
					'color': 'rgb(110, 110, 110)',
					'fontSize': 12,
					'fontStyle': 'normal',
					'fontWeight': 'normal',
					'fontFamily': 'sans-serif',
					'fill': '#fff'
				}
			},
			'axisTick': {
				'show': false,
				'symbol': 'line',
				'inside': false,
				'length': 10,
				'symbolStyle': {
					'stroke': '#fff',
					'stroke-width': 1
				}
			},
			'splitLine': {
				'show': false,
				'lineStyle': {
					'fill': 'none',
					'stroke': '#0f0',
					'stroke-width': 1,
					'type': 'dashed'
				}
			},
			'position': 'bottom',
			'min': 0,
			'max': 1500,
			'name': '',
			'nameLocation': '',
			'nameGap': '',
			'data': '',
			'boundaryGap': 1,
			'splitNumber': 5,
			'splitTicks': [

			],
			'splitArea': {
				'show': true,
				'areaStyle': {

				}
			}
		}
	],
	'yAxis': [
		{
			'type': 'category',
			'inverse': false,
			'axisLabel': {
				'show': true,
				'textStyle': {
					'fill': '#777'
				}
			},
			'axisLine': {
				'show': false,
				'lineStyle': {
					'fill': 'none',
					'stroke': '#777',
					'stroke-width': '2',
					'shape-rendering': 'crispEdges'
				}
			},
			'axisTick': {
				'show': false,
				'length': 10,
				'inside': false,
				'symbolStyle': {
					'stroke': '#000',
					'stroke-width': 1
				},
				'symbol': 'line'
			},
			'splitLine': {
				'show': false,
				'lineStyle': {
					'fill': 'none',
					'stroke': '#777',
					'stroke-width': 1
				}
			},
			'position': 'left',
			'data': [
				'类目1',
				'类目2',
				'类目3',
				'类目4',
				'类目5'
			],
			'name': '',
			'nameLocation': '',
			'nameGap': '',
			'min': '',
			'max': '',
			'boundaryGap': 1,
			'splitNumber': 5,
			'splitTicks': [

			],
			'splitArea': {
				'show': true,
				'areaStyle': {

				}
			}
		}
	],
	'series': [
		{
			'name': 'Apple',
			'type': 'tickbar',
			'coordinateSystem': 'cartesian2d',
			'data': [
				900,
				600,
				1100,
				800,
				1300
			],
			'clipPath': {
				'symbol': 'rect',
				'symbolGap': 0.1,
				'symbolNumber': 15,
				'showBackRect': true
			},
			'symbolStyle': {
				'normal': {
					'fill': 'rgb(41, 237, 138)',
					'borderColor': 'rgba(0, 0, 0, 0)',
					'borderWidth': 0,
					'borderType': 'none',
					'barBorderRadius': 0
				},
				'emphasis': {
					'fill': 'rgb(248, 234, 95)'
				},
				'backgroundColor': 'rgb(212, 251, 241)'
			},
			'label': {
				'position': 'maxRight',
				'textStyle': {
					'fill': 'rgb(122, 122, 122)',
					'fontSize': 12,
					'fontStyle': 'normal',
					'fontWeight': 'normal',
					'fontFamily': 'sans-serif',
					'font-size': '17px',
					'pointer-events': 'none'
				},
				'show': true,
				'symbol': 'text',
				'offsetX': 10,
				'offsetY': 0,
				'formatter': function formatter(param) {

	                return param.value;
	            }
			},
			'barWidth': 30,
			'barGap': 10
		}
	]
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Text |  | 控件类型——Text文本框，不可修改 |
| css | Object | √ |  |  | 文本框的样式 |
| css.width | String | √ | 100% | 支持CSS3中width的参数值 | 文本框的宽度 |
| css.height | String | √ | 100% | 支持CSS3中height的参数值 | 文本框的长度 |
| css.background | String | √ | none | 支持CSS3中background所有参数值 | 文本框的背景样式 |
| css.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 文本框中文本颜色 |
| css.fontFamily | String | √ | Hiragino Sans GB | 支持CSS3中font-family的 | 文本框中文本样式 |
| css.fontSize | String | √ | 20px | 支持CSS3中font-size的参数值 | 文本框中文本大小 |
| css.lineHeight | String | √ | 36px | 支持CSS3中line-height的参数值 | 文本框中文本的行间距 |
| css.borderWidth | String | √ | 2px | 支持CSS3中border-width的参数值 | 文本框的边框宽度 |
| css.borderRadius | String | √ | 5px | 支持CSS3中border-radius的参数值 | 文本框的边框圆角角度 |
| css.borderColor | String | √ | \#BCBCBC | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 文本框的边框颜色 |
| css.borderStyle | String | √ | solid | 支持CSS3中boder-style的参数值 | 文本框的边框样式 |
| css.textAlign | String | √ | left | 支持CSS3中text-align的参数值 | 文本框的文本水平对其方式 |
| text | String |  |  |  | 文本框中的文本内容 |

> 注：
>
> * CSS中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他文本框样式



