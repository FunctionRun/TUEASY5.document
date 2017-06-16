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


<table border="1">
    <tr>
        <th width="15%">配置项</th>
        <th width="30%">功能/描述</th>
        <th>可选参数</th>
    </tr>
    <tr>
        <td> type | String </td>
        <td>控件类型——singleCalendar时间，不可修改 </td>
        <td> singleCalendar </td>
    </tr>
    <tr>
        <td> themeColor | String</td>
        <td>日历界面的主体颜色</td>
        <td> \#667688 ('Color Name'、HEX、RGB、RGBA、HSL、HSLA、transparent ) </td>
    </tr>
    <tr>
        <td> itemStyle | Object </td>
        <td>显示条的样式</td>
        <td>Button</td>
    </tr>
    <tr>
        <td> itemStyle.inputStyle | Object</td>
        <td>显示条中日期显示框的样式 </td>
        <td><pre>
            {
                'color': '#333',
                'fontSize': '18px'
            }
        </pre></td>
    </tr>
    <tr>
        <td> itemStyle.selectStyle </td>
        <td> 显示条中日期筛选框（年、月、日的切换）的样式  </td>
        <td><pre>
            {
                'color': '#333',
                'fontFamily': '微软雅黑',
                'fontSize': '18px'
            }
        </pre></td>
    </tr>
</table>

> 注：
>
> * itemStyle.inputStyle和itemStyle.selectStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他日历样式
> * 关于日历界面、日期显示条以及日期显示条中的日期显示文本框和日期筛选框如下图展示：

![](/assets/singleCalendar.png)

