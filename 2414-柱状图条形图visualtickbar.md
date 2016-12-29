# 开发模式——通用参数

---

针对柱状图/条形图/折线图/散点图/面积图这类具有坐标轴的2D图表的通用参数

### 整体参数列表

```
{
    'color': [...],
    'grid': [...],
    'tooltip': [...],
    'xAxis': [...],
    'yAxis': [...],
    'series': [...]
}
```

### 整体参数说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| color | Array\(String\) | √ |  |  | 数据项的默认颜色配置列表，数组元素为十六进制表示的颜色 |
| [grid](#grid) | Array\(Object\) | √ |  |  | 直角坐标系内的绘图网格 |
| [tooltip](#tooltip) | Object | √ |  |  | 提示框，鼠标悬浮交互式时的信息提示 |
| [xAxis](#xaxis) | Array\(Object\) | √ |  |  | 直角坐标系中横轴数组 |
| yAxis | Array\(Object\) | √ |  |  | 直角坐标系中纵轴数组 |
| series | Array\(Object\) | √ |  |  | 该图表的详细配置 |

* ### grid

**参数配置列表**

```
'grid': [
        {
            'top': 10,
            'right': 50,
            'bottom': 20,
            'left': 50,
            'bgStyle': {
                'normal': {
                    'fill': 'rgba(0,0,0,0)'
                },
                'emphasis': {
                    'fill': 'rgba(0,0,0,0)'
                }
            }
        }
    ]
```

**参数字段说明**

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| grid\[0\].top | Number | √ | 10 |  | 直角坐标系内绘图网格左上角横坐标，数值单位px |
| grid\[0\].right | Number | √ | 50 |  | 直角坐标系内绘图网格左上角纵坐标，数值单位px |
| grid\[0\].bottom | Number | √ | 20 |  | 直角坐标系内绘图网格右下角纵坐标，数值单位px |
| grid\[0\].left | Number | √ | 50 |  | 直角坐标系内绘图网格右下角横坐标，数值单位px |
| grid\[0\].bgStyle | Object | √ |  |  | 直角坐标系内平面样式 |
| grid\[0\].bgStyle.normal | Object | √ |  |  | **未选中**状态的平面样式 |
| grid\[0\].bgStyle.normal.fill | String | √ | rgba\(0,0,0,0\) |  | **未选中**状态的平面填充颜色 |
| grid\[0\].bgStyle.emphasis | Object | √ |  |  | **选中**状态的平面样式 |
| grid\[0\].bgStyle.emphasis.fill | String | √ | rgba\(0,0,0,0\) |  | **选中**状态的平面填充颜色 |

* ### tooltip

**参数配置列表**

```
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
    }
```

**参数字段说明**

|  |  |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  |  |  |  |  |  |

* ### xAxis

**参数配置列表**

```
'xAxis': [
        {
            'type': 'linear',
            'inverse': false,
            'axisLine': {
                'show': false,
                'lineStyle': {
                    'stroke': 'yellow',
                    'stroke-width': '2'
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
                    'font-size': 12,
                    'font-style': 'normal',
                    'font-weight': 'normal',
                    'font-family': 'sans-serif',
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
```

**参数字段说明**

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| xAxis\[0\].type | String | √ | linear | category、linear |  |
| xAxis\[0\].inverse | Bool | √ | false |  | 是否沿水平方向反转图表 |
| xAxis\[0\].axisLine | Object | √ |  |  | 水平坐标轴线 |
| xAxis\[0\].axisLine.show | Bool | √ | false |  | 是否显示水平坐标轴线。 |
| xAxis\[0\].axisLine.lineStyle | Object | √ |  |  | 水平坐标轴线样式 |
| xAxis\[0\].axisLine.lineStyle.stroke | String | √ |  |  | 水平坐标轴线颜色 |
| xAxis\[0\].axisLine.lineStyle.stroke-width | String | √ | 2 |  | 水平坐标轴线宽度 |
| xAxis\[0\].axisLabel | Object | √ |  |  | 水平坐标轴文本标签 |
| xAxis\[0\].axisLabel.show | Bool | √ | false |  | 是否显示水平坐标轴文本标签 |
| xAxis\[0\].axisLabel.interval | String \| Number | √ | auto |  | 文本标签间隔。auto-自动隐藏显示不下的；0-全部显示 |
| xAxis\[0\].axisLabel.inside | Bool | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.rotate | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.margin | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.formatter | String \| Function | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.textStyle | Object | √ |  |  | 文本标签中的文本样式 |
| xAxis\[0\].axisLabel.textStyle.font-size | Number | √ | 12 |  | 文本标签中的文本大小 |
| xAxis\[0\].axisLabel.textStyle.font-style | String | √ | normal |  | 文本标签中的文本样式 |
| xAxis\[0\].axisLabel.textStyle.font-weight | String | √ | normal |  | 文本标签中的文本粗细 |
| xAxis\[0\].axisLabel.textStyle.font-family | String | √ | sans-serif |  | 文本标签中的文本字体 |
| xAxis\[0\].axisLabel.textStyle.fill | String | √ | \#fff |  | 文本标签中的文本颜色 |



