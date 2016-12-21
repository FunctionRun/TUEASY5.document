# 雷达\_ScanningRadar

---

> ## 开发模式

### 参数配置列表

```
{
    'scanningRadar': {
        'splitLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#0afea4'
            }
        },
        'axisLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#0afea4'
            }
        }
    },
    'series': [
        {
            'type': 'scanningRadar',
            'colors': [
                'white',
                '#10a7ba',
                'white'
            ]
        }
    ]
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| scanningRadar | Object | √ |  |  | 雷达底图样式 |
| scanningRadar.splitLine | Object | √ |  |  | 雷达底图圆环样式 |
| scanningRadar.splitLine.show | Bool | √ | true |  | 是否显示雷达底图圆环 |
| scanningRadar.splitLine.lineStyle | Object | √ |  |  | 雷达底图圆环线样式 |
| scanningRadar.splitLine.lineStyle.stroke | String | √ | \#0afea4 |  | 雷达底图圆环线颜色 |
| scanningRadar.axisLine | Object |  |  |  | 雷达底图辅助线 |
| scanningRadar.axisLine.show | Bool | √ | true |  | 是否显示雷达底图辅助线 |
| scanningRadar.axisLine.lineStyle | Object | √ |  |  | 雷达底图辅助线样式 |
| scanningRadar.axisLine.lineStyle.stroke | String | √ | \#0afea4 |  | 雷达底图辅助线颜色 |
| series | Array\(Object\) | √ |  |  | 雷达扫描片配色样式 |
| series\[0\].type | String | √ | scanningRadar |  | 控件类型——scanningRadar雷达，不可修改 |
| series\[0\].colors | String | √ | 'white','\#10a7ba','white' |  | 雷达扫描片配色组 |

> 注：
>
> * normal.imageStyle和normal.textStyle、mouse.imageStyle和mouse.textStyle、emphasis.imageStyle和emphasis.textStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他图片样式



