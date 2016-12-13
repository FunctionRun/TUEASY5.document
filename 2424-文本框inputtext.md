# 文本框\_Inputtext ![](/assets/inputtext.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Text',
    'label': {
        'text': '标签',
        'style': {
            'normal': {
                'textAlign': 'center',
                'fontSize': '16',
                'fontWeight': 400,
                'color': '#ccc'
            }
        }
    },
    'input': {
        'value': '',
        'style': {
            'normal': {
                'color': '#fff',
                'boxSizing': 'border-box',
                'borderRadius': '1',
                'fontSize': '15',
                'textAlign': 'center',
                'background': 'none',
                'borderBottom': '1px solid #4285F4'
            },
            'mouse': {
                'color': '#fff',
                'boxSizing': 'border-box',
                'borderRadius': '1',
                'fontSize': '16',
                'textAlign': 'center',
                'background': 'none',
                'border': '1px solid #4285F4'
            },
            'emphasis': {
                'color': '#fff',
                'boxSizing': 'border-box',
                'borderRadius': '1',
                'fontSize': '15',
                'textAlign': 'center',
                'background': 'none',
                'border': '1px solid #4285F4'
            }
        }
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Text |  | 控件类型——Text文本框，不可修改 |
| label | Object | √ |  |  | 文本框的提示标签 |
| label.text | String | √ | 标签 |  | 文本框的提示标签的文本内容 |
| label.style | Object | √ |  |  | 文本框的提示标签的样式 |
| label.style.normal | Object | √ |  |  | 文本框的提示标签的样式 |
| label.style.normal.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 文本框的提示标签的文本水平对其方式 |
| label.style.normal.fontSize | String | √ | 16px | 支持CSS3中font-size的参数值 | 文本框的提示标签的文本大小 |
| label.style.normal.fontWeight | String | √ | 400 | 支持CSS3中font-weight的参数值 | 文本框的提示标签的文本粗细 |
| label.style.normal.color | String | √ | \#ccc | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 文本框的提示标签的文本颜色 |
| input | Object | √ |  |  | 文本框的输入框 |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



