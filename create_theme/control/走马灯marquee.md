# 走马灯\_Marquee ![](/assets/Marquee.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Marquee',
    'series': [
        {
            'date': '2016.9.2',
            'time': '12:28:39',
            'content': '渝北区邮政银行遭遇抢劫'
        },
        {
            'date': '2016.9.2',
            'time': '22:28:39',
            'content': '渝北区珠宝店有小偷进入'
        },
        {
            'date': '2016.9.2',
            'time': '23:28:39',
            'content': '人民大街发生车祸'
        },
        {
            'name': '车辆轨迹',
            'value': 'carInfo'
        },
        {
            'name': '人员密度',
            'value': 'personIdentity'
        },
        {
            'name': '路况',
            'value': 'roadInfo'
        }
    ],
    'categoryGap': '80px',
    'itemGap': '20px',
    'speedTime': 20,
    'speedDistance': '2px',
    'itemStyle': {
        'normal': {
            'fontSize': '20px',
            'color': '#c1c1c1',
            'background': '#eff1f3',
            'paddingLeft': '5px'
        }
    }
}
```

### 参数字段说明

<table border="1" >
    <tr>
        <th width="15%">配置项</th>
        <th width="45%">功能/描述</th>
        <th>可选参数</th>
    </tr>
    <tr>
        <td>type | String</td>
        <td>控件类型——Marquee跑马灯，不可修改</td>
        <td>Marquee</td>
    </tr>
    <tr>
        <td>series | Array\(Object\)</td>
        <td>跑马灯控件中的数据项 </td>
        <td> <pre>
            [
                {
                    'name': '人员密度',
                    'value': 'personIdentity'
                }
            ]
        </pre> </td>
    </tr>
    <tr>
        <td>series\[0\].name | String</td>
        <td>数据文本内容，可以重复 </td>
        <td>'text'</td>
    </tr>
    <tr>
        <td>series\[0\].value | String</td>
        <td>数据唯一标识，不可重复 </td>
        <td>'id'</td>
    </tr>
    <tr>
        <td>categoryGap | String </td>
        <td>数据条之间的间距 </td>
        <td> 'px' or '%' </td>
    </tr>
    <tr>
        <td>itemGap | Sting </td>
        <td>一条数据的数据项之间的间距 </td>
        <td> 'px' or '%' </td>
    </tr>
    <tr>
        <td>speedTime | Number </td>
        <td>时间，单位毫秒 </td>
        <td> 20 </td>
    </tr>
    <tr>
        <td>speedDistance | String </td>
        <td>距离 </td>
        <td> 'px' or '%' </td>
    </tr>
    <tr>
        <td>itemStyle.normal | Object</td>
        <td>跑马灯控件的样式 </td>
        <td><pre>
            
            {
                //文本颜色，支持CSS3中颜色的参数值
                'fontSize': '20px',  
                //文本大小，支持CSS3中font-size的参数值
                'color': '#c1c1c1',  
                //背景颜色，支持CSS3中颜色的参数值
                'background': '#eff1f3',  
                //内左边距，支持CSS3中距离的参数值
                'paddingLeft': '5px'  
            }

        </pre></td>
    </tr>

</table>

> 注：
>
> * 跑马灯尚未绑定数据时，可以对series\[0\].data进行编辑；跑马灯绑定数据后，series会自动生成相应信息，可根据相应需求进行数据改动
> * 跑马灯的滑动速率由speedTime和speedDistance决定，单位时间内\(speedTime\)跑马灯走过的像素\(speedDistance\)
> * itemStyle.normal中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他跑马灯样式
> * 对于categoryGap和itemGap的区别如下图所示：

![](/assets/marquee01.png)

