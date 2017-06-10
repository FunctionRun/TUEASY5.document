# 时间\_SingleCalendar ![](/assets/Clock.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'singleCalendar',
    'themeColor': '#667688',
    'itemStyle': {
        'inputStyle': {
            'color': '#333',
            'fontSize': '18px'
        },
        'selectStyle': {
            'color': '#333',
            'fontFamily': '微软雅黑',
            'fontSize': '18px'
        }
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | singleCalendar |  | 控件类型——singleCalendar时间，不可修改 |
| themeColor | String | √ | \#667688 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 日历界面的主体颜色 |
| itemStyle | Object | √ |  |  | 显示条的样式 |
| itemStyle.inputStyle | Object | √ |  |  | 显示条中日期显示框的样式 |
| itemStyle.inputStyle.color | String | √ | \#333 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 显示条中日期显示框文本颜色 |
| itemStyle.inputStyle.fontSize | String | √ | 18px | 支持CSS3中font-size的参数值 | 显示条中日期显示框文本大小 |
| itemStyle.selectStyle | Object | √ |  |  | 显示条中日期筛选框（年、月、日的切换）的样式 |
| itemStyle.selectStyle.color | String | √ | \#333 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 显示条中日期筛选框文本颜色 |
| itemStyle.selectStyle.fontFamily | String | √ | 微软雅黑 | 支持CSS3中font-family的参数值 | 显示条中日期筛选框文本样式 |
| itemStyle.selectStyle.fontSize | String | √ | 18px | 支持CSS3中font-size的参数值 | 显示条中日期筛选框文本大小 |

> 注：
>
> * itemStyle.inputStyle和itemStyle.selectStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他日历样式
> * 关于日历界面、日期显示条以及日期显示条中的日期显示文本框和日期筛选框如下图展示：

![](/assets/singleCalendar.png)

