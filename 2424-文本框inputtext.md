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
                'display': 'inline-block',
                'textAlign': 'center',
                'padding': '0 10px',
                'verticalAlign': 'middle',
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
| label.style.normal | Object | √ |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



