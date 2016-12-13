# 选项框\_MultiCheckBox ![](/assets/MultiCheckBox.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'MultiCheckbox',
    'orient': 'horizontal',
    'itemGap': '10px',
    'iconGap': '5px',
    'series': [
        {
            'name': '选项一',
            'value': 'caseInfo'
        },
        {
            'name': '选项二',
            'value': 'police'
        },
        {
            'name': '选项三',
            'value': 'monitor'
        }
    ],
    'checkedValues': [
        'police',
        'caseInfo'
    ],
    'itemStyle': {
        'normal': {
            'color': '#999999',
            'fontSize': '20px',
            'backgroundColor': '#fff'
        },
        'checked': {
            'color': '#ffa84e',
            'fontSize': '20px'
        }
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | MultiCheckBox |  | 控件类型——MultiCheckBox选项框，不可修改 |
| orient | String | √ | horizontal | horizontal、vertical | 选项框方向。horizontal水平方向；vertical垂直方向 |
| itemGap | String | √ | 10px |  | 选项之间的间隔 |
| iconGap | String | √ | 5px |  | 选项的勾选框与选项文本框之间的间隔 |
| series | Array\(Object\) | √ |  |  | 选项数据 |
| series.name | String | √ |  |  | 选项文本内容，可以重复 |
| series.value | String | √ |  |  | 选项唯一标识，不可重复 |
| checkedValues | Array\(String\) | √ |  |  | 当前为选中状态下的选项标识 |
| itemStyle | Object | √ |  |  | 选项样式 |
| itemStyle.normal | Object | √ |  |  | 选项**未选中**状态样式 |
| itemStyle.normal.color | String | √ | \#999999 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 选项**未选中**状态勾选框与选项文本框内的文本颜色 |
| itemStyle.normal.fontSize | String | √ | 20px | 支持CSS3中font-size的参数值 | 选项**未选中**状态勾选框与选项文本框内的文本大小 |
| itemStyle.normal.backgroundColor | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 选项**未选中**状态勾选框与选项文本框内的背景颜色 |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



