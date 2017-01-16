# 图片\_Picture ![](/assets/Picture-icon.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Image',
    'selected': false,
    'normal': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px',
            'marginLeft': 0,
            'marginTop': 0
        }
    },
    'mouse': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px',
            'marginLeft': 0,
            'marginTop': 0
        }
    },
    'emphasis': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px'
        }
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Image |  | 控件类型——Image图片，不可修改 |
| selected | Bool | √ | false |  | 图片是否为选中状态 |
| normal | Object | √ |  |  | 图片**未选中**状态样式 |
| normal.src | String | √ |  |  | 图片**未选中**状态资源地址 |
| normal.text | String |  |  |  | 图片**未选中**状态的文本内容 |
| normal.imageStyle | Object | √ |  |  | 图片**未选中**状态图片样式 |
| normal.imageStyle.borderRadius | String | √ | 1px |  | 图片**未选中**状态的边框圆角角度 |
| normal.imageStyle.opacity | Number | √ | 0.0-1.0 |  | 图片**未选中**状态的透明度 |
| normal.textStyle | Object | √ |  |  | 图片**未选中**状态的文本样式 |
| normal.textStyle.color | String | √ | \#ccc | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 图片**未选中**状态的文本颜色 |
| normal.textStyle.fontSize | String | √ | 14px |  | 图片**未选中**状态的文本样子 |
| normal.textStyle.marginLeft | String | √ | -21 |  | 图片**未选中**状态的文本框左外边距 |
| normal.textStyle.marginTop | String | √ | -7 |  | 图片**未选中**状态的文本框上外边距 |
| mouse | Object | √ |  |  | 图片**鼠标悬浮**状态样式 |
| mouse.src | String | √ |  |  | 图片**鼠标悬浮**状态资源地址 |
| mouse.text | String |  |  |  | 图片**鼠标悬浮**状态的文本内容 |
| mouse.imageStyle | Object | √ |  |  | 图片**鼠标悬浮**状态图片样式 |
| mouse.imageStyle.borderRadius | String | √ | 1px |  | 图片**鼠标悬浮**状态的边框圆角角度 |
| mouse.imageStyle.opacity | Number | √ | 0.0-1.0 |  | 图片**鼠标悬浮**状态的透明度 |
| mouse.textStyle | Object | √ |  |  | 图片**鼠标悬浮**状态的文本样式 |
| mouse.textStyle.color | String | √ | \#ccc | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 图片**鼠标悬浮**状态的文本颜色 |
| mouse.textStyle.fontSize | String | √ | 14px |  | 图片**鼠标悬浮**状态的文本样子 |
| mouse.textStyle.marginLeft | String | √ | 0 |  | 图片**鼠标悬浮**状态的文本框左外边距 |
| mouse.textStyle.marginTop | String | √ | 0 |  | 图片**鼠标悬浮**状态的文本框上外边距 |
| emphasis | Object | √ |  |  | 图片**选中**状态样式 |
| emphasis.src | String | √ |  |  | 图片**选中**状态资源地址 |
| emphasis.text | String |  |  |  | 图片**选中**状态的文本内容 |
| emphasis.imageStyle | Object | √ |  |  | 图片**选中**状态图片样式 |
| emphasis.imageStyle.borderRadius | String | √ | 1px |  | 图片**选中**状态的边框圆角角度 |
| emphasis.imageStyle.opacity | Number | √ | 0.0-1.0 |  | 图片**选中**状态的透明度 |
| emphasis.textStyle | Object | √ |  |  | 图片**选中**状态的文本样式 |
| emphasis.textStyle.color | String | √ | \#ccc | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 图片**选中**状态的文本颜色 |
| emphasis.textStyle.fontSize | String | √ | 14px |  | 图片**选中**状态的文本样子 |

> 注：
>
> * normal.imageStyle和normal.textStyle、mouse.imageStyle和mouse.textStyle、emphasis.imageStyle和emphasis.textStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他图片样式



