# 时间\_MultiCalendar ![](/assets/MultiCalendar.png)

---
![](/assets/MultiCanendar01.png)
![](/assets/MultiCanendar02.png)
![](/assets/MultiCanendar03.png)
![](/assets/MultiCanendar04.png)
## 开发模式

### 参数配置列表

```
{
    'type': 'multiCalendar',
    'themeColor': '#667688',
    'orient': 'vertical',
    'inputStyle': {
        'color': '#333',
        'fontSize': '20px',
        'fontFamily': 'simsun'
    },
    'buttonStyle': {
        'normal': {
            'backgroundColor': '#33b26e',
            'color': 'white',
            'fontSize': '18px',
            'width': '100px'
        },
        'emphsis': {
            'backgroundColor': 'violet',
            'color': 'cyan',
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
        <td>multiCalendar </td>
    </tr>
    <tr>
        <td> themeColor | String </td>
        <td>日历界面的主体颜色 </td>
        <td> \#667688 ('Color Name'、HEX、RGB、RGBA、HSL、HSLA、transparent ) </td>
    </tr>
    <tr>
        <td> orient | String </td>
        <td>日历展示方式。horizontal横向展示、vertical纵向展示 </td>
        <td>vertical (horizontal、vertical) </td>
    </tr>
    <tr>
        <td> inputStyle | Object </td>
        <td>日期显示框的样式 </td>
        <td><pre>
            {
                'color': '#333',
                'fontSize': '20px',
                'fontFamily': 'simsun'
            }
        </pre></td>
    </tr>
    <tr>
        <td>buttonStyle | Object </td>
        <td>确认按钮样式  </td>
        <td> </td>
    </tr>
    <tr>
        <td>buttonStyle.normal | Object </td>
        <td>确认按钮**普通**状态样式 </td>
        <td><pre>
            {
                'backgroundColor': '#33b26e',
                'color': 'white',
                'fontSize': '18px',
                'width': '100px'
            }
        </pre></td>
    </tr>
    <tr>
        <td> buttonStyle.emphsis </td>
        <td> 确认按钮**鼠标悬浮**状态样式 </td>
        <td><pre>
            {
                'backgroundColor': 'violet',
                'color': 'cyan',
                'fontSize': '18px'
            }
        </pre></td>
    </tr>
</table>

> 注：
>
> * inputStyle和buttonStyle.normal、buttonStyle.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他日历样式



