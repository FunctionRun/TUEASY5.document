# 文本框\_Inputtext ![](/assets/inputtext.png)

---
> ## 小白编辑

### 参数字段说明

#### 选中
| 配置项 | 默认值  | 功能/备注 |
| :--- | :--- | :--- | 
| 标签文本 | 标签 |  文本框的提示标签的文本内容   | 
| 标签颜色 | #ccc |   文本框的提示标签的颜色  | 
| 标签大小 | 16px |   文本框的提示标签的大小  | 
| 输入字体值 |  |   文本框的输入框的文本值  | 
| 输入字体颜色 | #333 |  文本框的输入框的未选中状态文本颜色   | 
| 输入字体大小 | 15px |  文本框的输入框的未选中状态文本大小   | 
| 输入字体大小 | solid |  文本框的输入框的未选中状态文本框边框类型   | 
| 输入字体大小 | 1px |  文本框的输入框的未选中状态文本框边框宽度   | 
| 输入字体大小 | #4285F4 |  文本框的输入框的未选中状态文本框边框颜色   | 
| 输入字体大小 | 1 |  文本框的输入框的未选中状态文本框边框圆角   | 


#### 选中
| 配置项 | 默认值  | 功能/备注 |
| :--- | :--- | :--- | 
| 输入字体颜色 | #333 |  文本框的输入框的选中状态文本颜色   | 
| 输入字体大小 | 15px |  文本框的输入框的选中状态文本大小   | 
| 输入字体大小 | solid |  文本框的输入框的选中状态文本框边框类型   | 
| 输入字体大小 | 1px |  文本框的输入框的选中状态文本框边框宽度   | 
| 输入字体大小 | #4285F4 |  文本框的输入框的选中状态文本框边框颜色   | 
| 输入字体大小 | 1 |  文本框的输入框的选中状态文本框边框圆角   | 

#### 悬浮
| 配置项 | 默认值  | 功能/备注 |
| :--- | :--- | :--- | 
| 输入字体颜色 | #333 |  文本框的输入框的选中状态文本颜色   | 
| 输入字体大小 | 15px |  文本框的输入框的悬浮状态文本大小   | 
| 输入字体大小 | solid |  文本框的输入框的悬浮状态文本框边框类型   | 
| 输入字体大小 | 1px |  文本框的输入框的悬浮状态文本框边框宽度   | 
| 输入字体大小 | #4285F4 |  文本框的输入框的悬浮状态文本框边框颜色   | 
| 输入字体大小 | 1 |  文本框的输入框的悬浮状态文本框边框圆角   | 

 ## 开发模式

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
                'borderRadius': '1',
                'fontSize': '15',
                'textAlign': 'center',
                'background': 'none',
                'borderBottom': '1px solid #4285F4'
            },
            'mouse': {
                'color': '#fff',
                'borderRadius': '1',
                'fontSize': '16',
                'textAlign': 'center',
                'background': 'none',
                'border': '1px solid #4285F4'
            },
            'emphasis': {
                'color': '#fff',
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

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Text |  | 控件类型——Text文本框，不可修改 |
| label | Object | √ |  |  | 文本框的提示标签 |
| label.text | String | √ | 标签 |  | 文本框的提示标签的文本内容 |
| label.style | Object | √ |  |  | 文本框的提示标签的样式 |
| label.style.normal | Object | √ |  |  | 文本框的提示标签的样式 |
| label.style.normal.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 文本框的提示标签的文本水平对齐方式 |
| label.style.normal.fontSize | Number | √ | 16 |  | 文本框的提示标签的文本大小 |
| label.style.normal.fontWeight | String | √ | 400 | 支持CSS3中font-weight的参数值 | 文本框的提示标签的文本粗细 |
| label.style.normal.color | String | √ | \#ccc | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 文本框的提示标签的文本颜色 |
| input | Object | √ |  |  | 文本框的输入框 |
| input.value | String |  |  |  | 文本框的输入框文本内容 |
| input.style | Object | √ |  |  | 文本框的输入框的样式 |
| input.style.normal | Object | √ |  |  | 文本框的输入框的**未选中**状态样式 |
| input.style.normal.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 文本框的输入框的**未选中**状态文本颜色 |
| input.style.normal.borderRadius | Number | √ | 1 |  | 文本框的输入框的**未选中**状态文本框圆角角度 |
| input.style.normal.fontSize | fontSize | √ | 15 |  | 文本框的输入框的**未选中**状态文本大小 |
| input.style.normal.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 文本框的输入框的**未选中**状态文本水平对齐方式 |
| input.style.normal.background | String | √ | none | 支持CSS3中background所有参数值 | 文本框的输入框的**未选中**状态文本框背景 |
| input.style.normal.borderColor | String | √ | \#4285F4 | 颜色值| 文本框的输入框的**未选中**状态文本框边框颜色|
| input.style.normal.borderWidth | Number | √ | 1 | 支持CSS3中border-bottom的参数值 | 文本框的输入框的**未选中**状态文本框边框底边样式宽度 |
| input.style.normal.borderStyle | String | √ |  solid | 支持CSS3中border-bottom的参数值 | 文本框的输入框的**未选中**状态文本框边框底边样式 |
| input.style.mouse | Object | √ |  |  | 文本框的输入框的**鼠标悬浮**状态样式 |
| input.style.mouse.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 文本框的输入框的**鼠标悬浮**状态文本颜色 |
| input.style.mouse.borderRadius | Number | √ | 1 |  | 文本框的输入框的**鼠标悬浮**状态文本框圆角角度 |
| input.style.mouse.fontSize | Number | √ | 16 | 支持CSS3中font-size的参数值 | 文本框的输入框的**鼠标悬浮**状态文本大小 |
| input.style.mouse.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 文本框的输入框的**鼠标悬浮**状态文本水平对齐方式 |
| input.style.mouse.background | String | √ | none | 支持CSS3中background所有参数值 | 文本框的输入框的**鼠标悬浮**状态文本框背景 |
| input.style.mouse.border | String | √ | 1px solid \#4285F4 | 支持CSS3中border的参数值 | 文本框的输入框的**鼠标悬浮**状态文本框边框样式 |
| input.style.emphasis | Object | √ |  |  | 文本框的输入框的**选中**状态样式 |
| input.style.emphasis.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 文本框的输入框的**选中**状态文本颜色 |
| input.style.emphasis.borderRadius | Number | √ | 1 |  | 文本框的输入框的**选中**状态文本框圆角角度 |
| input.style.emphasis.fontSize | Numer | √ | 15 |  | 文本框的输入框的**选中**状态文本大小 |
| input.style.emphasis.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 文本框的输入框的**选中**状态文本水平对齐方式 |
| input.style.emphasis.background | String | √ | none | 支持CSS3中background所有参数值 | 文本框的输入框的**选中**状态文本框背景 |
| input.style.normal.borderColor | String | √ | \#4285F4 | 颜色值| 文本框的输入框的**选中**状态文本框边框颜色|
| input.style.normal.borderWidth | Number | √ | 1 | 支持CSS3中border-bottom的参数值 | 文本框的输入框的**选中**状态文本框边框底边样式宽度 |
| input.style.normal.borderStyle | String | √ |  solid | 支持CSS3中border-bottom的参数值 | 文本框的输入框的**选中**状态文本框边框底边样式 |

> 注：
>
> * style.normal、style.mouse、style.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他文本框样式



