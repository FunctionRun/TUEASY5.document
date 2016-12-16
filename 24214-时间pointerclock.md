# 时间\_PionterClock ![](/assets/Clock.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'clock': {
        'clockAxis': {
            'axisLine': {
                'show': true,
                'lineStyle': {
                    'stroke': '#5a9cc7'
                }
            },
            'axisTick': {
                'show': true,
                'lineStyle': {
                    'stroke': '#5a9cc7'
                }
            },
            'axisText': {
                'textGap': 5,
                'textStyle': {
                    'fill-opacity': 0.8,
                    'fill': '#5a9cc7',
                    'stroke': '#5a9cc7'
                }
            }
        },
        'outerCircle': {
            'show': true,
            'lineStyle': {
                'fill': '#5a9cc7'
            }
        },
        'hand': {
            'clockHourHand': {
                'handStyle': {
                    'fill': '#5a9cc7',
                    'stroke': '#5a9cc7'
                },
                'lineStyle': {
                    'stroke': '#5a9cc7'
                }
            },
            'clockMinuteHand': {
                'handStyle': {
                    'fill': '#5a9cc7',
                    'stroke': '#5a9cc7'
                },
                'lineStyle': {
                    'fill': '#5a9cc7'
                }
            },
            'clockSecondHand': {
                'handStyle': {
                    'fill': '#5a9cc7'
                },
                'lineStyle': {
                    'fill': '#5a9cc7'
                }
            }
        },
        'aloneArc': {
            'show': true,
            'lineStyle': {
                'fill': '#5a9cc7',
                'stroke': '#5a9cc7'
            }
        },
        'symmetryArc': {
            'show': true,
            'lineStyle': {
                'fill': '#5a9cc7',
                'stroke': '#5a9cc7'
            }
        },
        'solidLineImmediatelyDottedLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#5a9cc7'
            }
        },
        'solidLineInsideDottedLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#5a9cc7'
            }
        }
    },
    'series': [
        {
            'type': 'PointerClock'
        }
    ]
}
```

### 参数字段说明

![](/assets/pointerClock01.png)

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| clock | Object | √ |  |  | 钟表样式 |
| clock.clockAxis | Object | √ |  |  | 钟表刻度辅助样式 |
| clock.clockAxis.axisLine | Object | √ |  |  | 钟表刻度辅助圆线样式 |
| clock.clockAxis.axisLine.show | Bool | √ | true |  | 是否显示钟表刻度辅助圆线 |
| clock.clockAxis.axisLine.lineStyle | Object | √ |  |  | 钟表刻度辅助圆线样式 |
| clock.clockAxis.axisLine.lineStyle.stroke | String | √ | \#5a9cc7 |  | 钟表刻度辅助圆线颜色 |
| clock.clockAxis.axisTick | Object | √ |  |  | 钟表的辅助刻度线样式 |
| clock.clockAxis.axisTick.show | Bool | √ | true |  | 是否显示钟表的辅助刻度线 |
| clock.clockAxis.axisTick.lineStyle | Object | √ |  |  | 钟表的辅助刻度线样式 |
| clock.clockAxis.axisTick.lineStyle.stroke | String | √ | \#5a9cc7 |  | 钟表的辅助刻度线颜色 |
| clock.clockAxis.axisTick | Object | √ |  |  | 钟表的辅助刻度线样式 |
| clock.clockAxis.axisTick.show | Bool | √ | true |  | 是否显示钟表的辅助刻度线 |
| clock.clockAxis.axisTick.lineStyle | Object | √ |  |  | 钟表的辅助刻度线样式 |
| clock.clockAxis.axisTick.lineStyle.stroke | String | √ | \#5a9cc7 |  | 钟表的辅助刻度线颜色 |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



