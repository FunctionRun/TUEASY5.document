# 导航\_withTriangleNav ![](/assets/withTriangleNav.png)

---

> ## 绑定数据

* 用户绑定数据前，需要事先保存页面

![](/assets/withTriangleNav01.png)

* 该控件所绑定的数据为文本数据，导航栏中会列出选中维度中的数据内容并删除重复内容

* 对绑定的数据进行一些其他配置包括：筛选数据条数、定时刷新时间、推送数据接口

* 绑定数据结束后，进行数据配置保存，返回控件编辑界面

![](/assets/withTriangleNav02.png)

> ## 用户配置

* 点击编辑参数按钮，默认进入开发模式参数配置，点击设置按钮进入用户配置面板

![](/assets/withTriangleNav03.png)

* 控件的未选中状态配置：文本设置、背景设置、边框设置

![](/assets/withTriangleNav04.png)

> 注：
>
> 1.当边框勾选项为选中状态，可进行边框设置。
>
> 2.该控件边框设置中的圆角设置为禁用。

* 控件的选中状态配置

![](/assets/withTriangleNav05.png)

> 注：三角形长度设置（标6）是指等腰直角三角形的直角边长度设定，该值可改变三角形标志大小。



> ## 开发者配置

>
## 开发模式

### 参数配置列表

```
	{
    'currentSelect': 0,
    'automatic': {
        'start': false,
        'interval': 2000
    },
    'maxNumInOneLine': 100,
    'series': [{
        'type': 'withTriangle',
        'data': [{
            'key': 'create',
            'name': '创业'
        }, {
            'key': 'map',
            'name': '地图'
        }, {
            'key': 'police',
            'name': '交警'
        }, {
            'key': 'managerPolice',
            'name': '城管'
        }, {
            'key': 'fire',
            'name': '消防'
        }],
        'textStyle': {
            'normal': {
                'fontSize': '18px',
                'color': '#667688'
            },
            'emphasis': {
                'fontSize': '18px',
                'color': '#fff'
            }
        },
        'borderStyle': {
            'normal': {
                'borderWidth': '1px',
                'borderStyle': 'solid',
                'borderColor': '#fff',
                'borderRadius': '1px'
            }
        },
        'backgroundStyle': {
            'normal': {
                'backgroundColor': 'rgba(239, 241, 243, 1.0)',
                'backgroundSize': 'cover'
            },
            'emphasis': {
                'backgroundColor': 'rgba(102, 118, 136, 1.0)',
                'backgroundSize': 'cover'
            }
        },
        'tiangleStyle': {
            'normal': {
                'border': 'none'
            },
            'emphasis': {
                'borderWidth': '10px',
                'borderStyle': 'solid',
                'borderTopColor': '#ffa84e',
                'borderRightColor': '#ffa84e'
            }
        }
    }],
    'itemGap': '30',
}
```

### 参数字段说明
<table border="1">
<tr>
<th width="15%">配置项</th>
<th width="50%">功能/描述</th>
<th>可选参数</th>
</tr>
<tr>
<td>currentSelect | Number</td>
<td>初始化进入导航栏时默认的当前选中项</td>
<td></td>
</tr>
<tr>
<td>automatic | Object</td>
<td>自动切换导航栏，有start和interval两个属性</td>
<td></td>
</tr>
<tr>
<td>automatic.start | Bool</td>
<td>是否自动切换导航栏</td>
<td></td>
</tr>
<tr>
<td>automatic.interval | Number</td>
<td>切换导航项的时间间隔，单位为毫秒。该属性当且仅当start为true时有效</td>
<td></td>
</tr>
<tr>
<td>maxNumInOneLine | Number</td>
<td>导航栏中每行可以显示最多的导航项数目</td>
<td></td>
</tr>
<tr>
<td>series | Array[Object]</td>
<td>数据及样式的系列配置</td>
<td></td>
</tr>
<tr>
<td>series[0].type | String</td>
<td>控件类型——withTriangleNav导航栏，不可修改</td>
<td>withTriangle</td>
</tr>
<tr>
<td>series[0].data | Array[Object]</td>
<td>导航控件中的数据项</td>
<td></td>
</tr>
<tr>
<td>series[0].data[0].key | String</td>
<td>导航项数据的唯一标识，不可重复</td>
<td></td>
</tr>
<tr>
<td>series[0].data[0].name | String</td>
<td>导航项显示的文本数据信息，允许重复</td>
<td></td>
</tr>
<tr>
<td>series[0].textStyle | Object</td>
<td>导航项的文本样式，有normal和emphasis两个属性</td>
<td></td>
</tr>
<tr>
<td>series[0].textStyle.normal | Object</td>
<td>导航项<b>未选中</b>状态下的文本样式</td>
<td><pre> {
//文本大小，支持CSS3中font-size的参数值
'fontSize': '18px',
//文本颜色，支持CSS3中颜色的参数值
'color': '#667688'
}</pre></td>
</tr>
<tr>
<td>series[0].textStyle.emphasis | Object</td>
<td>导航项<b>选中</b>状态下的文本样式</td>
<td><pre> {
//文本大小，支持CSS3中font-size的参数值
'fontSize': '18px',
//文本颜色，支持CSS3中颜色的参数值
'color': '#fff'
}</pre></td>
</tr>
<tr>
<td>series[0].borderStyle | Object</td>
<td>导航项的边框样式，仅有normal一个属性</td>
<td></td>
</tr>
<tr>
<td>series[0].borderStyle.normal | Object</td>
<td>导航项边框样式</td>
<td><pre> {
//边框宽度，支持CSS3中border-width的参数值
'borderWidth': '1px',
//边框样式，支持CSS3中boder-style的参数值
'borderStyle': '#solid',
//边框颜色，支持CSS3中颜色的参数值
'borderColor': '#fff',
//边框圆角角度，支持CSS3中border-radius的参数值
'borderRadius': '1px'
}</pre></td>
</tr>
<tr>
<td>series[0].backgroundStyle | Object</td>
<td>导航项的背景样式，有normal和emphasis两个属性</td>
<td></td>
</tr>
<tr>
<td>series[0].backgroundStyle.normal | Object</td>
<td>导航项<b>未选中</b>状态下的背景样式</td>
<td><pre> {
//背景颜色，支持CSS3中颜色的参数值
'backgroundColor': 'rgba(239, 241, 243, 1.0)',
//背景大小，支持CSS3中background-size的参数值
'backgroundSize': 'cover'
}</pre></td>
</tr>
<tr>
<td>series[0].backgroundStyle.emphasis | Object</td>
<td>导航项<b>选中</b>状态下的背景样式</td>
<td><pre> {
//背景颜色，支持CSS3中颜色的参数值
'backgroundColor': 'rgba(239, 241, 243, 1.0)',
//背景大小，支持CSS3中background-size的参数值
'backgroundSize': 'cover'
}</pre></td>
</tr>
<tr>
<td>series[0].triangleStyle | Object</td>
<td>导航项的三角标志样式，有normal和emphasis两个属性</td>
<td></td>
</tr>
<tr>
<td>series[0].triangleStyle.normal | Object</td>
<td>导航项<b>未选中</b>状态下的三角标志样式<b>不显示</b>，不可修改该属性</td>
<td><pre> {
'border': 'none'
}</pre></td>
</tr>
<tr>
<td>series[0].triangleStyle.emphasis | Object</td>
<td>导航项<b>选中</b>状态下的三角标志样式</td>
<td><pre> {
//等腰直角三角形的直角边长，决定三角标志的大小
//支持CSS3中border-width的参数值
'borderWidth': '10px',
//三角标志的上三角颜色，支持CSS3中颜色的参数值
'borderTopColor': '#ffa84e',
//三角标志的下三角颜色，支持CSS3中颜色的参数值
'borderRightColor': '#ffa84e'
}</pre></td>
</tr>
<tr>
<td>series[0].name | String</td>
<td>导航栏绑定数据时的数据字段名称</td>
<td></td>
</tr>
<tr>
<td>itemGap | Number</td>
<td>导航项之间的间距</td>
<td></td>
</tr>
</table>



> 注：
>
> * 导航栏尚未绑定数据时，可以对series\[0\].data进行编辑；导航栏绑定数据后，series\[0\].data会自动生成相应信息，用户只可以对name值进行修改
> * textStyle两种状态下的文本样式均支持CSS3中的文本样式，命名采用驼峰命名方式，用户可按照规则添加其他文本样式
> * borderStyle两种状态下的文本样式均支持CSS3中的边框样式，命名采用驼峰命名方式，用户可按照规则添加其他边框样式
> * backgroundStyle两种状态下的背景样式均支持CSS3中的文本样式，命名采用驼峰命名方式，用户可按照规则添加其他文本样式

| borderTopColor和borderRightColor取值相同 | borderTopColor和borderRightColor取值不同 |
| :---: | :---: |
| ![](/assets/withTriangleNav_icon1.png) | ![](/assets/withTriangleNav_icon2.png) |



