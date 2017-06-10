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

<table border="1">
<tr>
	<th width="15%">配置项</th>
	<th width="30%">功能/描述</th>
	<th>可选参数</th>
</tr>
<tr>
	<td>type | String</td>
	<td>控件类型——Weather自定义，不可修改</td>
	<td>Weather</td>
</tr>
<tr>
	<td>weatherControlStyle | Object</td>
	<td>天气控件的整体样式</td>
	<td><pre> {
	//背景样式，支持CSS3中background的参数值
	'background': '#ccc'
}</pre></td>
</tr>
<tr>
	<td>getWeather | Object</td>
	<td>天气控件的天气信息获取及显示样式</td>
	<td><pre> {
	//宽度，支持CSS3中width的参数值
	'width': '300px',
	//高度，支持CSS3中height的参数值
	'height': '300px',
	...
}</pre></td>
</tr>
<tr>
	<td>getWeather.isByCity | Object</td>
	<td>天气控件通过城市名获取天气信息，有byCity和city两个属性</td>
	<td><pre> {
	//是否通过城市名获取天气信息，Bool
	'byCity': 'true',
	//获取天气信息的城市名，String
	'city': '北京'
}</pre></td>
</tr>
<tr>
	<td>getWeather.isByCoordinates | Object</td>
	<td>天气控件通过经纬度名获取天气信息，有byCoordinates、longitude和latitude三个属性</td>
	<td><pre> {
	//是否通过经纬度获取天气信息，Bool
	'byCoordinates': 'true',
	//获取天气信息的经度，String
	'longitude': '116.305145',
	//获取天气信息的纬度，String
	'latitude': '39.982368'
}</pre></td>
</tr>
<tr>
	<td>getWeather.windStyle | Object</td>
	<td>天气控件中<b>风</b>信息样式</td>
	<td><pre> {
	//文本样式
	'textStyle': {
		//文本颜色，支持CSS3中颜色的参数值
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.weatherStyle | Object</td>
	<td>天气控件中<b>天气</b>信息样式</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.temperatureStyle | Object</td>
	<td>天气控件中<b>温度</b>信息样式</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.timeStyle | Object</td>
	<td>天气控件中<b>时间</b>信息样式</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.weekStyle | Object</td>
	<td>天气控件中<b>星期</b>信息样式</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
</table>

> 注：
>
> * weatherControlStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他天气样式
> * getWeather.windStyle.textSryle、getWeather.weatherStyle.textSryle、getWeather.temperatureStyle.textSryle、getWeather.timeStyle.textSryle、getWeather.weekStyle.textSryle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他天气信息样式



