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
| series\[0\].data | Array\[Object\] | √ |  |  | 导航控件中的数据项 |
| series\[0\].data\[0\].key | String | √ |  |  | 导航项的唯一标识，不可重复 |
| series\[0\].data\[0\].name | String | √ |  |  | 导航项显示的文本信息，允许重复 |
| series\[0\].textStyle | Object | √ |  |  | 导航项的文本样式 |
| series\[0\].textStyle.normal | Object | √ |  |  | 导航项**未选中**状态下的文本样式 |
| series\[0\].textStyle.normal.fontSize | String | √ | 18px | 支持CSS3中font-size的参数值 | 导航项**未选中**状态下的文本大小 |
| series\[0\].textStyle.normal.color | String | √ | \#ffa84e | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**未选中**状态下的文本颜色 |
| series\[0\].textStyle.emphasis | Object | √ |  |  | 导航项**选中**状态下的文本样式 |
| series\[0\].textStyle.emphasis.fontSize | String | √ | 18px | 支持CSS3中font-size的参数值 | 导航项**选中**状态下的文本大小 |
| series\[0\].textStyle.emphasis.color | String | √ | \#ffa84e | 支持CSS3中颜色的值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**选中**状态下的文本颜色 |
| series\[0\].backgroundPathStyle | Object | √ |  |  | 导航项的背景斜线样式 |
| series\[0\].backgroundPathStyle.normal | Object | √ |  |  | 导航项**未选中**状态下的背景斜线样式 |
| series\[0\].backgroundPathStyle.normal.stroke | String | √ | \#ffe3c6 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**未选中**状态下的背景斜线的颜色 |
| series\[0\].backgroundPathStyle.normal.opacity | Number | √ | 0 | 0.0-1.0 | 导航项**未选中**状态下的背景斜线的透明度 |
| series\[0\].backgroundPathStyle.emphasis | Object | √ |  |  | 导航项**选中**状态下的背景斜线样式 |
| series\[0\].backgroundPathStyle.emphasis.stroke | String | √ | \#ffe3c6 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航项**选中**状态下的背景斜线的颜色 |
| series\[0\].backgroundPathStyle.emphasis.opacity | Number | √ | 1 | 0.0-1.0 | 导航项**选中**状态下的背景斜线的透明度 |
| series\[0\].bothSidesStyle | Object | √ |  |  | 导航项的左右边框样式 |
| series\[0\].bothSidesStyle.normal | Object | √ |  |  | 导航框**未选中**状态的左右边框样式 |
| series\[0\].bothSidesStyle.normal.borderColor | String | √ | \#ffd3a6 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航框**未选中**状态的左右边框颜色 |
| series\[0\].bothSidesStyle.emphasis | Object | √ |  |  | 导航框**选中**状态的左右边框样式 |
| series\[0\].bothSidesStyle.emphasis.borderColor | String | √ | \#f6eb3f | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 导航框**选中**状态的左右边框颜色 |
| series\[0\].name | String |  |  |  | 导航栏绑定数据时的数据字段 |
| itemGap | Number | √ | 24 |  | 导航项之间的间距 |

> 注：
>
> * 导航栏尚未绑定数据时，可以对series\[0\].data进行编辑;导航栏绑定数据后，series\[0\].data会自动生成相应信息，用户只可以对name值进行修改
> * textStyle两种状态下的文本样式均支持CSS3中的文本样式，命名采用驼峰命名方式，用户可按照规则添加其他文本样式



