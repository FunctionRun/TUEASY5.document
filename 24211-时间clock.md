# 时间\_Clock ![](/assets/Clock.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'time': {
        'secondShow': false,
        'normal': {
            'color': '#616a73',
            'fontSize': '50px',
            'line-height': '30px',
            'position': 'absolute',
            'left': 55,
            'top': 16
        }
    },
    'date': {
        'normal': {
            'color': '#84b0ed',
            'fontSize': '18px',
            'position': 'absolute',
            'left': 19,
            'top': 70
        }
    },
    'week': {
        'normal': {
            'color': '#84b0ed',
            'fontSize': '18px',
            'position': 'absolute',
            'right': 21,
            'top': 70
        }
    },
    'border': {
        'show': true,
        'normal': {
            'borderColor': '#85bbbd'
        }
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| time | Object | √ |  |  | 时间信息及样式 |
| time.secondShow | Bool | √ | false |  | 时间单位是够精确显示到秒 |
| time.normal | Object | √ |  |  | 时间样式 |
| time.normal.color | String | √ | \#616a73 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 时间信息文本颜色 |
| time.normal.fontSize | String | √ | 50px | 支持CSS3中font-size的参数值 | 时间信息文本大小 |
| time.normal.left | String | √ | 55px |  | 时间信息文本左外边距边界与其包含块左边界之间的间距 |
| time.normal.top | String | √ | 16px |  | 时间信息文本上外边距边界与其包含块上边界之间的间距 |
| date | Object | √ |  |  | 日期信息及样式 |
| date.normal | Object | √ |  |  | 日期样式 |
| date.normal.color | String | √ | \#616a73 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 日期信息文本颜色 |
| date.normal.fontSize | String | √ | 50px | 支持CSS3中font-size的参数值 | 日期信息文本大小 |
| date.normal.left | String | √ | 55px |  | 日期信息文本左外边距边界与其包含块左边界之间的间距 |
| date.normal.top | String | √ | 16px |  | 日期信息文本上外边距边界与其包含块上边界之间的间距 |
| week | Object | √ |  |  | 星期信息及样式 |
| week.normal | Object | √ |  |  | 星期样式 |
| week.normal.color | String | √ | \#616a73 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 星期信息文本颜色 |
| week.normal.fontSize | String | √ | 50px | 支持CSS3中font-size的参数值 | 星期信息文本大小 |
| week.normal.left | String | √ | 55px |  | 星期信息文本左外边距边界与其包含块左边界之间的间距 |
| week.normal.top | String | √ | 16px |  | 星期信息文本上外边距边界与其包含块上边界之间的间距 |
| border | Object | √ |  |  | 边框样式 |
| border.show | Bool | √ | fase |  | 是否显示边框 |
| border.normal | Object | √ |  |  | 边框样式，当且仅当border.show的值为true时有效 |
| border.normal.borderColor | String | √ | \#85bbbd | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 边框颜色 |

> 注：
>
> * border.normal中的属性支持CSS3中的边框样式属性，命名采用驼峰命名方式，用户可按照规则添加其他边框样式



