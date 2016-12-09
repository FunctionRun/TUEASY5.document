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
        'animationType': 'lattice',
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
                    'borderColor': '#ffd3a6',
                    'background': '#ffd3a6'
                },
                'emphasis': {
                    'borderColor': '#f6eb3f',
                    'background': '#f6eb3f'
                }
            }
        }
    ],
    'itemGap': '24',
    'a': {

    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| currentSelect | Number | √ | 0 |  | 初始化进入导航栏时默认的当前选中项 |
| automatic | Object | √ |  |  | 自动切换导航栏 |
| automatic.start | Bool | √ | false |  | 是否自动切换导航栏 |
| automatic.interval | Number |  |  |  | 切换导航项的时间间隔，单位为毫秒。该属性当且仅当start为true时有效。 |
| maxNumInOneLine | Number | √ | 100 |  | 一行导航栏中可以显示最多的导航项数目 |
| animation | Object | √ |  |  | 鼠标悬浮在导航项时的动画效果 |
| animation.showAnimation | Bool | √ | true |  | 是否应用动画效果 |
| animation.animationType | String | √ | lattice |  | 动画效果样式 |
| animation.animationDelay | Number | √ | 1000 |  | 动画延时时间，即鼠标悬浮后与动画开始时间间隔，单位毫秒 |
| series | Array\[Object\] | √ |  |  | 数据及样式的系列配置 |
| series\[0\].type | String | √ | withLines |  | 控件类型——linesNav导航栏，不可修改 |
| series\[0\].data | Array\[Object\] | √ |  |  | 导航控件所有数据 |
| series\[0\].data\[0\].key | String | √ |  |  | 导航项的唯一标识，不可重复 |
| series\[0\].data\[0\].name | String | √ |  |  | 导航项显示的文本信息，允许重复 |
| series\[0\].textStyle | Object | √ |  |  | 导航项的文本样式 |
| series\[0\].textStyle.normal | Object | √ |  |  | 导航项**未选中**状态下的文本样式 |
| series\[0\].textStyle.normal.fontSize | String | √ | 18px |  | 导航项**未选中**状态下的文本大小 |
| series\[0\].textStyle.normal.color | String | √ | \#ffa84e | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**未选中**状态下的文本颜色 |
| series\[0\].textStyle.emphasis | Object | √ |  |  | 导航项**选中**状态下的文本样式 |
| series\[0\].textStyle.emphasis.fontSize | String | √ | 18px |  | 导航项**选中**状态下的文本大小 |
| series\[0\].textStyle.emphasis.color | String | √ | \#ffa84e | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**选中**状态下的文本颜色 |
| series\[0\].backgroundPathStyle | Object | √ |  |  | 导航项的背景斜线样式 |
| series\[0\].backgroundPathStyle.normal | Object | √ |  |  | 导航项**未选中**状态下的背景斜线样式 |
| series\[0\].backgroundPathStyle.normal.stroke | String | √ | \#ffe3c6 | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**未选中**状态下的背景斜线的颜色 |
| series\[0\].backgroundPathStyle.normal.opacity | Number | √ | 0 | 0.0-1.0 | 导航项**未选中**状态下的背景斜线的透明度 |
| series\[0\].backgroundPathStyle.emphasis | Object | √ |  |  | 导航项**选中**状态下的背景斜线样式 |
| series\[0\].backgroundPathStyle.emphasis.stroke | String | √ | \#ffe3c6 | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**选中**状态下的背景斜线的颜色 |
| series\[0\].backgroundPathStyle.emphasis.opacity | Number | √ | 1 | 0.0-1.0 | 导航项**选中**状态下的背景斜线的透明度 |
| series\[0\].backgroundStyle | Object | √ |  |  | 导航项的背景样式 |
| series\[0\].backgroundStyle.normal | Object | √ |  |  | 导航项**未选中**状态下的背景样式 |
| series\[0\].backgroundStyle.normal.backgroundColor | String | √ | rgba\(239, 241, 243, 1.0\) | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**未选中**状态下的背景颜色 |
| series\[0\].backgroundStyle.normal.backgroundSize | String | √ | cover | 支持CSS3中background-size的参数值 | 导航项**未选中**状态下的背景图像尺寸 |
| series\[0\].backgroundStyle.emphasis | Object | √ |  |  | 导航项**未选中**状态下的背景样式 |
| series\[0\].backgroundStyle.emphasis.backgroundColor | String | √ | rgba\(102, 118, 136, 1.0\) | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**选中**状态下的背景颜色 |
| series\[0\].backgroundStyle.emphasis.backgroundSize | String | √ | cover | 支持CSS3中background-size的参数值 | 导航项**选中**状态下的背景图像尺寸 |
| series\[0\].triangleStyle | Object | √ |  |  | 导航项的三角标志样式 |
| series\[0\].triangleStyle.normal | Object | √ | { ’border‘: 'none' } |  | 导航项在**未选中**状态下不显示三角标志，不可修改 |
| series\[0\].triangleStyle.emphasis | Object | √ |  |  | 导航项在**选中**状态下的三角标志样式 |
| series\[0\].triangleStyle.emphasis.borderWidth | String | √ | 10px |  | 等腰直角三角形的直角边长，决定三角标志的大小 |
| series\[0\].triangleStyle.emphasis.borderTopColor | String | √ | \#ffa84e | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 三角标志的上三角颜色 |
| series\[0\].triangleStyle.emphasis.borderRightColor | String | √ | \#ffa84e | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 三角标志的下三角颜色 |
| series\[0\].name | String |  |  |  | 导航栏绑定数据时的数据字段 |
| itemGap | Number | √ | 24 |  | 导航项之间的间隔 |



