# 按钮\_basicButton ![](/assets/basicButton.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Button',
    'normal': {
        'backgroundColor': '#31b16c',
        'fontSize': '20',
        'borderRadius': '5',
        'border': '1px solid #31b16c',
        'color': '#fff',
        'lineHeight': '30px',
        'textAlign': 'center',
        'cursor': 'pointer',
        'opacity': 0.6
    },
    'mouse': {
        'backgroundColor': '#31b16c',
        'borderRadius': '5',
        'fontSize': '20',
        'border': '1px solid #31b16c',
        'color': '#fff',
        'lineHeight': '30px',
        'textAlign': 'center',
        'cursor': 'pointer',
        'opacity': 0.8
    },
    'emphasis': {
        'backgroundColor': '#31b16c',
        'borderRadius': '5',
        'fontSize': '20',
        'color': '#fff',
        'lineHeight': '30px',
        'textAlign': 'center',
        'border': '1px solid #31b16c',
        'opacity': 0.7
    },
    'selected': false,
    'text': '确 认'
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Button |  | 控件类型——Button按钮，不可修改 |
| normal | Object | √ |  |  | 按钮**未选中**状态样式 |
| normal.backgroundColor | String | √ | \#31b16c | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 按钮**未选中**状态背景颜色 |
| normal.fontSize | String | √ | 20px | 支持CSS3中font-size的参数值 | 按钮**未选中**状态文本大小 |
| normal.borderRadius | String | √ | 5px | 支持CSS3中border-radius的参数值 | 按钮**未选中**状态边框圆角角度 |
| normal.border | String | √ | 1px solid \#31b16c | 支持CSS3中border的参数值 | 按钮**未选中**状态边框样式 |
| normal.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 按钮**未选中**状态文本颜色 |
| normal.lineHeight | String | √ | 30px | 支持CSS3中line-height的参数值 | 按钮**未选中**状态文本的行间距 |
| normal.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 按钮**未选中**状态文本水平对齐方式 |
| normal.cursor | String | √ | pointer | 支持CSS3中cursor的参数值 | 按钮**未选中**状态光标的类型 |
| normal.opacity | Number | √ | 0.6 | 0.0-1.0 | 按钮**未选中**状态背景透明度 |
| mouse | Object | √ |  |  | 按钮**鼠标悬浮**状态样式 |
| mouse.backgroundColor | String | √ | \#31b16c | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 按钮**鼠标悬浮**状态背景颜色 |
| mouse.fontSize | String | √ | 20px | 支持CSS3中font-size的参数值 | 按钮**鼠标悬浮**状态文本大小 |
| mouse.borderRadius | String | √ | 5px | 支持CSS3中border-radius的参数值 | 按钮**鼠标悬浮**状态边框圆角角度 |
| mouse.border | String | √ | 1px solid \#31b16c | 支持CSS3中border的参数值 | 按钮**鼠标悬浮**状态边框样式 |
| mouse.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 按钮**鼠标悬浮**状态文本颜色 |
| mouse.lineHeight | String | √ | 30px | 支持CSS3中line-height的参数值 | 按钮**鼠标悬浮**状态文本的行间距 |
| mouse.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 按钮**鼠标悬浮**状态文本水平对齐方式 |
| mouse.cursor | String | √ | pointer | 支持CSS3中cursor的参数值 | 按钮**鼠标悬浮**状态光标的类型 |
| mouse.opacity | Number | √ | 0.8 | 0.0-1.0 | 按钮**鼠标悬浮**状态背景透明度 |



