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

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Marquee |  | 控件类型——Marquee跑马灯，不可修改 |
| series | Array\(Object\) | √ |  |  | 跑马灯控件中的数据项 |
| series\[0\].name | String | √ |  |  | 数据文本内容，可以重复 |
| series\[0\].value | String | √ |  |  | 数据唯一标识，不可重复 |
| categoryGap | String | √ | 20px |  | 数据条之间的间距 |
| itemGap | Sting | √ | 10px |  | 一条数据的数据项之间的间距 |
| speedTime | Number | √ | 20 |  | 速率-时间，单位毫秒 |
| speedDistance | String | √ | 2px |  | 速率-距离 |
| itemStyle | Object | √ |  |  | 跑马灯控件的样式 |
| itemStyle.normal | Object | √ |  |  | 跑马灯控件的样式 |
| itemStyle.normal.fontSize | String | √ | 20px | 支持CSS3中font-size的参数值 | 跑马灯控件的文本大小 |
| itemStyle.normal.color | String | √ | \#c1c1c1 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 跑马灯控件的文本颜色 |
| itemStyle.normal.background | String | √ | \#eff1f3 | 支持CSS3中background的所有参数值 | 跑马灯控件的背景样式 |
| itemStyle.normal.paddingLeft | String | √ | 5px |  | 跑马灯控件的左内边距 |

> 注：
>
> * 跑马灯尚未绑定数据时，可以对series\[0\].data进行编辑；跑马灯绑定数据后，series会自动生成相应信息，可根据相应需求进行数据改动
> * 跑马灯的滑动速率由speedTime和speedDistance决定，单位时间内\(speedTime\)跑马灯走过的像素\(speedDistance\)
> * itemStyle.normal中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他跑马灯样式
> * 对于categoryGap和itemGap的区别如下图所示：

![](/assets/marquee01.png)

