# 表格\_Table ![](/assets/table.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Table',
    'width': '100%',
    'height': '100%',
    'tableStyle': {
        'borderWidth': 0,
        'borderStyle': 'solid',
        'borderColor': '#999',
        'textAlign': 'center',
        'width': '100%',
        'height': '100%'
    },
    'theadStyle': {
        'show': true,
        'normal': {
            'backgroundColor': '#667688',
            'color': '#fff'
        },
        'mouse': {
            'backgroundColor': '#445960',
            'color': '#fff'
        }
    },
    'theadTr': {
        'height': 40
    },
    'hoverable': 'cell',
    'tbodyTr': {
        'normal': {
            'backgroundColor': '#eff1f3',
            'height': NaN,
            'color': '#8c96a2'
        },
        'mouse': {
            'backgroundColor': '#ccc',
            'height': NaN,
            'color': '#8c96a2'
        }
    },
    'tdStyle': {
        'borderWidth': 2,
        'borderStyle': 'solid',
        'borderColor': '#fff',
        'font-size': '20px'
    },
    'index': {
        'show': true,
        'theadContent': '排名',
        'tbodyPrefix': 'NO.'
    },
    'series': {
        '列1': [
            1,
            2,
            3,
            4
        ],
        '列2': [
            1,
            2,
            3,
            4
        ]
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Table |  | 控件类型——Table表格，不可修改 |
| width | String | √ | 100% | 支持CSS3中width的参数值 | 表格的宽度 |
| height | String | √ | 100% | 支持CSS3中height的参数值 | 表格的长度 |
| tableStyle | Object | √ |  |  | 表格整体样式 |
| tableStyle.borderWidth | String | √ | 0 | 支持CSS3中border-width的参数值 | 表格边框宽度 |
| tableStyle.borderStyle | String | √ | solid | 支持CSS3中border-style的参数值 | 表格边框样式 |
| tableStyle.borderColor | String | √ | \#999 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表格边框颜色 |
| tableStyle.textAlign | String | √ | center | 支持CSS3中text-align的参数值 | 表格文本水平对其方式 |
| tableStyle.width | String | √ | 100% | 支持CSS3中width的参数值 | 表格内部宽度 |
| tableStyle.height | String | √ | 100% | 支持CSS3中height的参数值 | 表格内部高度 |
| theadStyle | Object | √ |  |  | 表格表头样式 |
| theadStyle.show | Bool | √ | true |  | 是否显示表头 |
| theadStyle.normal | Object | √ |  |  | 表头**未选中**状态样式 |
| theadStyle.normal.backgroundColor | String | √ | \#667688 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表头**未选中**状态背景颜色 |
| theadStyle.normal.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表头**未选中**状态文字颜色 |
| theadStyle.mouse | Object | √ |  |  | 表头**鼠标悬浮状**态样式 |
| theadStyle.mouse.backgroundColor | String | √ | \#445960 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表头**鼠标悬浮**状态背景颜色 |
| theadStyle.mouse.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表头**鼠标悬浮**状态文字颜色 |
| theadStyle.theadTr | String |  |  |  | 表头表格行样式 |
| theadStyle.theadTr.height | String | √ | 40px | 支持CSS3中height的参数值 | 表头表格行高度 |
| hoverable | String | √ | cell | 支持CSS3中:hover的参数值 | 选择鼠标指针浮动在表格上面的单元格 |
| tbodyTr | Object | √ |  |  | 表格表身行样式 |
| tbodyTr.normal | Object | √ |  |  | 表身行**未选中**状态样式 |
| tbodyTr.normal.backgroundColor | String | √ | \#eff1f3 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表身行**未选中**状态背景颜色 |
| tbodyTr.normal.color | String | √ | \#8c96a2 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表身行**未选中**状态文字颜色 |
| tbodyTr.mouse | Object | √ |  |  | 表身行**鼠标悬浮状**态样式 |
| tbodyTr.mouse.backgroundColor | String | √ | \#ccc | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表身行**鼠标悬浮**状态背景颜色 |
| tbodyTr.mouse.color | String | √ | \#8c96a2 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 表身行**鼠标悬浮**状态文字颜色 |
| tdStyle | Object | √ |  |  | 表格单元格样式 |
| tdStyle.borderWidth | String | √ | 2px | 支持CSS3中border-width的参数值 | 单元格边框宽度 |
| tdStyle.borderStyle | String | √ | solid | 支持CSS3中border-style的参数值 | 单元格边框样式 |
| tdStyle.borderColor | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 单元格边框颜色 |
| tdStyle.fontSize | String | √ | 20px | 支持CSS3中font-size的参数值 | 单元格文本字体大小 |
| index | Object | √ |  |  | 表格列提示 |
| index.show | Bool | √ |  |  | 是否显示表格列提示 |
| index.theadContent | String | √ |  |  | 表头中的表格列提示文本内容 |
| index.tbodyPrefix | String |  |  |  | 表身中列序号的共同前缀 |
| series | Object |  |  |  | 表格数据内容 |

> 注：
>
> * 表格尚未绑定数据时，series中的一个属性对应表格表头的一个单元格内容，其属性值（为Array数组类型）对应该单元格所在列的单元格内容；绑定数据后series会自动生成，用户可根据自己需求手动修改表格数据内容
> * tableStyle、theadStyle.normal和theadStyle.mouse、theadTr、tbodyTr.normal和tbodyTr.mouse、tdStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他表格样式

![](/assets/table01.png)

