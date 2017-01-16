# 时间\_PionterClock ![](/assets/PointerClock.png)

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
        'middleCircle': {
            'show': true,
            'lineStyle': {
                'stroke': '#5a9cc7'
            }
        },
        'innerCircle': {
            'show': true,
            'lineStyle': {
                'stroke': '#5a9cc7'
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
| clock.clockAxis.axisLine.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表刻度辅助圆线颜色 |
| clock.clockAxis.axisTick | Object | √ |  |  | 钟表的辅助刻度线样式 |
| clock.clockAxis.axisTick.show | Bool | √ | true |  | 是否显示钟表的辅助刻度线 |
| clock.clockAxis.axisTick.lineStyle | Object | √ |  |  | 钟表的辅助刻度线样式 |
| clock.clockAxis.axisTick.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的辅助刻度线颜色 |
| clock.clockAxis.axisText | Object | √ |  |  | 钟表的辅助数字盘样式 |
| clock.clockAxis.axisText.textGap | String | √ | 5px |  | 钟表的辅助数字盘与钟表中间圆边框的间距 |
| clock.clockAxis.axisText.textStyle | Object | √ |  |  | 钟表的辅助数字盘数字样式 |
| clock.clockAxis.axisText.textStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的辅助数字盘数字颜色 |
| clock.outerCircle | Object | √ |  |  | 钟表的外圆边框样式 |
| clock.outerCircle.show | Bool | √ | true |  | 是否显示钟表的外圆边框 |
| clock.outerCircle.lineStyle | Object | √ |  |  | 钟表的外圆边框样式 |
| clock.outerCircle.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的外圆边框颜色 |
| clock.middleCircle | Object | √ |  |  | 钟表的中间圆边框样式 |
| clock.middleCircle.show | Bool | √ | true |  | 是否显示钟表的中间圆边框 |
| clock.middleCircle.lineStyle | Object | √ |  |  | 钟表的中间圆边框样式 |
| clock.middleCircle.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的中间圆边框颜色 |
| clock.innerCircle | Object | √ |  |  | 钟表的内圆边框样式 |
| clock.innerCircle.show | Bool | √ | true |  | 是否显示钟表的内圆边框 |
| clock.innerCircle.lineStyle | Object | √ |  |  | 钟表的内圆边框样式 |
| clock.innerCircle.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的内圆边框颜色 |
| clock.hand | Object | √ |  |  | 钟表的指针样式 |
| clock.hand.clockHourHand | Object | √ |  |  | 钟表的时针样式 |
| clock.hand.clockHourHand.handStyle | Object | √ |  |  | 钟表时针的针柄样式 |
| clock.hand.clockHourHand.handStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表时针的针柄填充颜色 |
| clock.hand.clockHourHand.handStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表时针的针柄边框颜色 |
| clock.hand.clockHourHand.lineStyle | Object | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表时针的其余边框颜色 |
| clock.hand.clockMinuteHand | Object | √ |  |  | 钟表的分针样式 |
| clock.hand.clockMinuteHand.handStyle | Object | √ |  |  | 钟表分针的针柄样式 |
| clock.hand.clockMinuteHand.handStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表分针的针柄填充颜色 |
| clock.hand.clockMinuteHand.handStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表分针的针柄边框颜色 |
| clock.hand.clockMinuteHand.lineStyle | Object | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表分针的其余边框颜色 |
| clock.hand.clockSecondHand | Object | √ |  |  | 钟表的秒针样式 |
| clock.hand.clockSecondHand.handStyle | Object | √ |  |  | 钟表秒针的针柄样式 |
| clock.hand.clockSecondHand.handStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表秒针的针柄填充颜色 |
| clock.hand.clockSecondHand.lineStyle | Object | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表秒针的其余边框颜色 |
| clock.aloneArc | Object | √ |  |  | 钟表的单独弧线装饰 |
| clock.aloneArc.show | Bool | √ | true |  | 是否显示钟表的单独弧线 |
| clock.aloneArc.lineStyle | Object | √ |  |  | 钟表的单独弧线样式 |
| clock.aloneArc.lineStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的单独弧线填充颜色 |
| clock.aloneArc.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的单独弧线边框颜色 |
| clock.symmetryArc | Object | √ |  |  | 钟表的对称弧线装饰 |
| clock.symmetryArc.show | Bool | √ | true |  | 是否显示钟表的对称弧线 |
| clock.symmetryArc.lineStyle | Object | √ |  |  | 钟表的对称弧线样式 |
| clock.symmetryArc.lineStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的对称弧线填充颜色 |
| clock.symmetryArc.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 钟表的对称弧线边框颜色 |



