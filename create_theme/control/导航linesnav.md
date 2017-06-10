# 导航\_linesNav ![](/assets/linesNav.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'currentSelect': 0,
    'automatic': {
        'start': false,
        'interval': 2000
    },
    'maxNumInOneLine': 100,
    'animation': {
        'showAnimation': true,
        'animationType': 'withLines',
        'animationDelay': 1000
    },
    'orient': 'horizontal',
    'series': [
        {
            'type': 'lattice',
            'data': [
                {
                    'key': 'create',
                    'name': '创业'
                },
                {
                    'key': 'map',
                    'name': '地图'
                },
                {
                    'key': 'police',
                    'name': '交警'
                },
                {
                    'key': 'managerPolice',
                    'name': '城管'
                },
                {
                    'key': 'fire',
                    'name': '消防'
                }
            ],
            'textStyle': {
                'normal': {
                    'fontSize': '18px',
                    'color': '#ffa84e'
                },
                'emphasis': {
                    'fontSize': '18px',
                    'color': '#ffa84e'
                }
            },
            'backgroundPathStyle': {
                'normal': {
                    'color': '#ffe3c6',
                    'stroke': '#ffe3c6',
                    'opacity': 0
                },
                'emphasis': {
                    'stroke': '#ffe3c6',
                    'opacity': 1
                }
            },
            'bothSidesStyle': {
                'normal': {
                    'borderColor': '#ffd3a6'
                },
                'emphasis': {
                    'borderColor': '#f6eb3f'
                }
            }
        }
    ],
    'itemGap': '24'
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
<td>animation | Object</td>
<td>鼠标悬浮在导航项时的动画效果，有showAnimation、animationType和animationDelay三个属性</td>
<td></td>
</tr>
<tr>
<td>animation.showAnimation | Bool</td>
<td>是否应用动画效果</td>
<td></td>
</tr>
<tr>
<td>animation.animationType | String</td>
<td>动画效果样式</td>
<td>lattice</td>
</tr>
<tr>
<td>animation.animationDelay | Number</td>
<td>动画延时时间，即鼠标悬浮后与动画开始时间间隔，单位毫秒</td>
<td></td>
</tr>
<tr>
<td>orient | String</td>
<td>导航栏的布局方向</td>
<td>horizontal</td>
</tr>
<tr>
<td>series | Array[Object]</td>
<td>数据及样式的系列配置</td>
<td></td>
</tr>
<tr>
<td>series[0].type | String</td>
<td>控件类型——withTriangleNav导航栏，不可修改</td>
<td>withLines</td>
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
'color': '#ffa84e'
}</pre></td>
</tr>
<tr>
<td>series[0].textStyle.emphasis | Object</td>
<td>导航项<b>选中</b>状态下的文本样式</td>
<td><pre> {
'fontSize': '18px',
'color': '#ffa84e'
}</pre></td>
</tr>
<tr>
<td>series[0].backgroundPathStyle | Object</td>
<td>导航项的背景斜线，有normal和emphasis两个属性</td>
<td></td>
</tr>
<tr>
<td>series[0].backgroundPathStyle.normal | Object</td>
<td>导航项<b>未选中</b>状态下的背景斜线样式</td>
<td><pre> {
//背景斜线颜色，支持CSS3中颜色的参数值
'stroke': '#ffe3c6',
//背景斜线透明度，支持0.0至1.0的数值型参数值
'opacity': 0
}</pre></td>
</tr>
<tr>
<td>series[0].backgroundPathStyle.emphasis | Object</td>
<td>导航项<b>选中</b>状态下的背景斜线样式</td>
<td><pre> {
'stroke': '#ffe3c6',
'opacity': 1
}</pre></td>
</tr>
<tr>
<td>series[0].bothSidesStyle | Object</td>
<td>导航项的左右边框样式，有normal和emphasis两个属性</td>
<td></td>
</tr>
<tr>
<td>series[0].bothSidesStyle.normal | Object</td>
<td>导航项<b>未选中</b>状态下的左右边框样式</td>
<td><pre> {
//左右边框颜色，支持CSS3中颜色的参数值
'borderColor': '#ffd3a6'
}</pre></td>
</tr>
<tr>
<td>series[0].bothSidesStyle.emphasis | Object</td>
<td>导航项<b>选中</b>状态下的左右边框样式</td>
<td><pre> {
'borderColor': '#f6eb3f'
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




