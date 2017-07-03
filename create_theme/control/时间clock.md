# 时间\_Clock ![](/assets/Clock.png)

---

## 编辑模式
![](/assets/Clock01.png)
![](/assets/Clock03.png)
![](/assets/Clock04.png)
![](/assets/Clock05.png)
## 开发模式
![](/assets/Clock02.png)

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

<table border="1">
    <tr>
        <th width="15%">配置项</th>
        <th width="30%">功能/描述</th>
        <th>可选参数</th>
    </tr>
    <tr>
        <td>time | Object  </td>
        <td>时间信息及样式</td>
        <td> </td>
    </tr>
    <tr>
        <td>time.secondShow | Bool </td>
        <td>时间单位是够精确显示到秒</td>
        <td>false</td>
    </tr>
    <tr>
        <td>time.normal | Object </td>
        <td>时间样式</td>
        <td><pre>
            {
                'color': '#616a73',
                'fontSize': '50px',
                'line-height': '30px',
                'position': 'absolute',
                'left': 55,
                'top': 16
            }
        </pre></td>
    </tr>
    <tr>
        <td>date | Object </td>
        <td>日期信息及样式</td>
        <td> </td>
    </tr>
    <tr>
        <td>date.normal | Object </td>
        <td>日期样式</td>
        <td><pre>
            {
                'color': '#84b0ed',
                'fontSize': '18px',
                'position': 'absolute',
                'left': 19,
                'top': 70
            }
        </pre></td>
    </tr>
    <tr>
        <td>week | Object </td>
        <td>星期信息及样式</td>
        <td> </td>
    </tr>
    <tr>
        <td>week.normal | Object </td>
        <td>星期样式</td>
        <td><pre>
            {
                'color': '#84b0ed',
                'fontSize': '18px',
                'position': 'absolute',
                'right': 21,
                'top': 70
            }
        </pre></td>
    </tr>
    <tr>
        <td>border | Object </td>
        <td>边框样式</td>
        <td> </td>
    </tr>
    <tr>
        <td>border.show | Bool </td>
        <td>是否显示边框</td>
        <td>false</td>
    </tr>
    <tr>
        <td>border.normal | Object </td>
        <td>边框样式，当且仅当border.show的值为true时有效</td>
        <td><pre>
            {
                'borderColor': '#85bbbd'
            }
        </pre></td>
    </tr>
</table>

> 注：
>
> * border.normal中的属性支持CSS3中的边框样式属性，命名采用驼峰命名方式，用户可按照规则添加其他边框样式



