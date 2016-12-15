# 走马灯\_Marquee ![](/assets/Weather.png)

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
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



