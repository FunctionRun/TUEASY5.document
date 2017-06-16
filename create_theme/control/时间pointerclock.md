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

<table border="1">
    <tr>
        <th width="15%">配置项</th>
        <th width="30%">功能/描述</th>
        <th>可选参数</th>
    </tr>
    <tr>
        <td> clock | Object  </td>
        <td>钟表样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.clockAxis | Object  </td>
        <td>钟表刻度辅助样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisLine | Object </td>
        <td>钟表刻度辅助圆线样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisLine.show | Bool  </td>
        <td>是否显示钟表刻度辅助圆线 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisLine.lineStyle | Object </td>
        <td>钟表刻度辅助圆线样式 </td>
        <td><pre>
    {
        'stroke': '#5a9cc7'
    }
        </pre></td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisTick | Object  </td>
        <td>钟表的辅助刻度线样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisTick.show | Bool </td>
        <td>是否显示钟表的辅助刻度线 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisTick.lineStyle | Object </td>
        <td>钟表的辅助刻度线样式 </td>
        <td><pre>
    {
        'stroke': '#5a9cc7'
    }
        </pre></td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisText | Object </td>
        <td>钟表的辅助数字盘样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisText.textGap | String </td>
        <td>钟表的辅助数字盘与钟表中间圆边框的间距 </td>
        <td>'5px'</td>
    </tr>
    <tr>
        <td>clock.clockAxis.axisText.textStyle | Object </td>
        <td>钟表的辅助数字盘数字样式 </td>
        <td><pre>
    {
        'stroke': '#5a9cc7'
    }
        </pre></td>
    </tr>
    <tr>
        <td>clock.outerCircle | Object  </td>
        <td>钟表的外圆边框样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.outerCircle.show | Bool </td>
        <td>是否显示钟表的外圆边框 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>clock.outerCircle.lineStyle | Object </td>
        <td>钟表的外圆边框样式 </td>
        <td><pre>
    {
        'stroke': '#5a9cc7'
    }
        </pre></td>
    </tr>
    <tr>
        <td>clock.middleCircle | Object </td>
        <td>钟表的中间圆边框样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.middleCircle.show | Bool </td>
        <td>是否显示钟表的中间圆边框 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>clock.middleCircle.lineStyle | Object </td>
        <td>钟表的中间圆边框样式 </td>
        <td><pre>
    {
        'stroke': '#5a9cc7'
    }
        </pre></td>
    </tr>
    <tr>
        <td>clock.innerCircle | Object </td>
        <td>钟表的内圆边框样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.innerCircle.show | Bool </td>
        <td>是否显示钟表的内圆边框 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>clock.innerCircle.lineStyle | Object </td>
        <td>钟表的内圆边框样式 </td>
        <td><pre>
    {
        'stroke': '#5a9cc7'
    }
        </pre></td>
    </tr>
    <tr>
        <td>clock.hand | Object </td>
        <td>钟表的指针样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.hand.clockHourHand | Object </td>
        <td>钟表的时针样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.hand.clockHourHand.handStyle | Object </td>
        <td>钟表时针的针柄样式 </td>
        <td><pre>
{
    'fill': '#5a9cc7',
    'stroke': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td>clock.hand.clockHourHand.lineStyle | Object </td>
        <td>钟表时针的其余边框颜色 </td>
        <td><pre>
{
    'stroke': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td>clock.hand.clockMinuteHand | Object </td>
        <td>钟表的分针样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.hand.clockMinuteHand.handStyle | Object </td>
        <td>钟表分针的针柄样式 </td>
        <td><pre>
{
    'fill': '#5a9cc7',
    'stroke': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td>clock.hand.clockMinuteHand.lineStyle | Object </td>
        <td>钟表分针的其余边框颜色 </td>
        <td><pre>
{
    'fill': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td>clock.hand.clockSecondHand | Object </td>
        <td>钟表的秒针样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.hand.clockSecondHand.handStyle | Object </td>
        <td>钟表秒针的针柄样式 </td>
        <td><pre>
{
    'fill': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td>clock.hand.clockSecondHand.lineStyle | Object </td>
        <td>钟表秒针的其余边框颜色 </td>
        <td><pre>
{
    'fill': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td> clock.aloneArc | Object </td>
        <td>钟表的单独弧线装饰 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.aloneArc.show | Bool </td>
        <td>是否显示钟表的单独弧线 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>clock.aloneArc.lineStyle | Object </td>
        <td>钟表的单独弧线样式 </td>
        <td><pre>
{
    'fill': '#5a9cc7',
    'stroke': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td>clock.symmetryArc | Object </td>
        <td>钟表的对称弧线装饰 </td>
        <td> </td>
    </tr>
    <tr>
        <td>clock.symmetryArc.show | Bool </td>
        <td>是否显示钟表的对称弧线 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>clock.symmetryArc.lineStyle | Object </td>
        <td>钟表的对称弧线样式 </td>
        <td><pre>
{
    'fill': '#5a9cc7',
    'stroke': '#5a9cc7'
}
        </pre></td>
    </tr>
    <tr>
        <td> series | Array\(Object\)</td>
        <td>数据项 </td>
        <td> </td>
    </tr>
    <tr>
        <td> series\[0\].type | String</td>
        <td> 当前控件类型</td>
        <td>'PointerClock'</td>
    </tr>
</table>

![](/assets/pointerClock01.png)




