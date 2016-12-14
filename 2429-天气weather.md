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
| getWeather.isByCoordinates | Object | √ |  |  | 天气控件通过经纬度名获取天气信息 |
| getWeather.isByCoordinates.byCity | Bool | √ | true |  | 是否通过经纬度获取天气信息 |
| getWeather.isByCoordinates.longitude | String | √ | 116.305145 |  | 获取天气信息的经度 |
| getWeather.isByCoordinates.latitude | String | √ | 39.982368 |  | 获取天气信息的维度 |
| getWeather.windStyle | Object | √ |  |  | 天气控件中**风**信息样式 |
| getWeather.windStyle.textStyle | Object | √ |  |  | 天气控件中**风**信息文本样式 |
| getWeather.windStyle.textStyle.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 天气控件中**风**信息文本颜色 |
| getWeather.weatherStyle | Object | √ |  |  | 天气控件中**天气**信息样式 |
| getWeather.weatherStyle.textStyle | Object | √ |  |  | 天气控件中**天气**信息文本样式 |
| getWeather.weatherStyle.textStyle.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 天气控件中**天气**信息文本颜色 |
| getWeather.temperatureStyle | Object | √ |  |  | 天气控件中**温度**信息样式 |
| getWeather.temperatureStyle.textStyle | Object | √ |  |  | 天气控件中**温度**信息文本样式 |
| getWeather.temperatureStyle.textStyle.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 天气控件中**温度**信息文本颜色 |
| getWeather.timeStyle | Object | √ |  |  | 天气控件中**时间**信息样式 |
| getWeather.timeStyle.textStyle | Object | √ |  |  | 天气控件中**时间**信息文本样式 |
| getWeather.timeStyle.textStyle.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 天气控件中**时间**信息文本颜色 |
| getWeather.timeStyle | Object | √ |  |  | 天气控件中**时间**信息样式 |
| getWeather.timeStyle.textStyle | Object | √ |  |  | 天气控件中**时间**信息文本样式 |
| getWeather.timeStyle.textStyle.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 天气控件中**时间**信息文本颜色 |


