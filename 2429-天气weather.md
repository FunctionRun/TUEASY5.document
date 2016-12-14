# 天气\_Weather ![](/assets/Weather.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Weather',
    'weatherControlStyle': {
        'background': '#ccc'
    },
    'getWeather': {
        'width': '300px',
        'height': '300px',
        'isByCity': {
            'byCity': true,
            'city': '北京'
        },
        'isByCoordinates': {
            'byCooordinates': false,
            'longitude': '116.305145',
            'latitude': '39.982368'
        },
        'windStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'weatherStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'temperatureStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'timeStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'weekStyle': {
            'textStyle': {
                'color': '#fff'
            }
        }
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Weather |  | 控件类型——Weather天气，不可修改 |
| weatherControlStyle | Object | √ |  |  | 天气控件的整体样式 |
| weatherControlStyle.background | String | √ | \#ccc | 支持CSS3中background的所有参数值 | 天气控件的背景样式 |
| getWeather | Object | √ |  |  | 天气控件的天气信息获取及显示样式 |
| getWeather.width |  |  |  |  |  |
| getWeather.height |  |  |  |  |  |
| getWeather.isByCity | Object | √ |  |  | 天气控件通过城市名获取天气信息 |
| getWeather.isByCity.byCity | Bool | √ | true |  | 是否通过城市名获取天气信息 |
| getWeather.isByCity.city | String | √ | 北京 |  | 获取天气信息的城市名 |
| getWeather.isByCity.byCity | Bool | √ | true |  | 是否通过城市名获取天气信息 |
| getWeather.isByCity.city | String | √ | 北京 |  | 获取天气信息的城市名 |



