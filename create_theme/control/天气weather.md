# 天气\_Weather ![](/assets/Weather.png)

---

> ## 开发模式

### 参数配置列表

```
{
	'type': 'Weather',
	'width': '100%',
	'height': '100%',
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
			'color': '#dedede'
		}
	},
	'weatherStyle': {
		'textStyle': {
			'color': '#dedede'
		}
	},
	'temperatureStyle': {
		'textStyle': {
			'color': '#dedede'
		}
	},
	'timeStyle': {
		'textStyle': {
			'color': '#dedede'
		}
	},
	'weekStyle': {
		'textStyle': {
			'color': '#dedede'
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
	<td> isByCity | Object</td>
	<td> Get data by city name </td>
	<td><pre> 
{
  'byCity': true,
  'city': '北京'
}</pre></td>
</tr>
<tr>
	<td> isByCoordinates | Object</td>
	<td> Get data by Cooordinates </td>
	<td><pre> 
 {
   'byCooordinates': false,
   'longitude': '116.305145',
   'latitude': '39.982368'
 } </pre></td>
</tr>
<tr>
	<td> windStyle | Object</td>
	<td> Wind style </td>
	<td><pre> 
 {
   'textStyle': {
      'color': '#dedede'
   }
 } </pre></td>
</tr>
<tr>
	<td> weatherStyle | Object</td>
	<td> Weather style </td>
	<td><pre> 
 {
   'textStyle': {
      'color': '#dedede'
   }
 } </pre></td>
</tr>
<tr>
	<td> temperatureStyle | Object</td>
	<td> Temperatures style </td>
	<td><pre> 
 {
   'textStyle': {
      'color': '#dedede'
   }
 } </pre></td>
</tr>
<tr>
	<td> timeStyle | Object</td>
	<td> Time style </td>
	<td><pre> 
 {
   'textStyle': {
      'color': '#dedede'
   }
 } </pre></td>
</tr>
<tr>
	<td> weekStyle | Object</td>
	<td> Week style </td>
	<td><pre> 
 {
   'textStyle': {
      'color': '#dedede'
   }
 } </pre></td>
</tr>
</table>

> 注：
>
> * weatherControlStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他天气样式
> * getWeather.windStyle.textSryle、getWeather.weatherStyle.textSryle、getWeather.temperatureStyle.textSryle、getWeather.timeStyle.textSryle、getWeather.weekStyle.textSryle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他天气信息样式



