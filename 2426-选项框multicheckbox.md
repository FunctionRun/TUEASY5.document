# 选项框\_MultiCheckBox ![](/assets/MultiCheckBox.png)

---
> ## 小白编辑

### 参数字段说明

#### 选中
| 配置项 | 默认值  | 功能/备注 |
| :--- | :--- | :--- | 
| 显示内容（逗号隔开） | 选项一,选项二,选项三 |  选择框的选项内容   | 
| 初始化选中内容 |police,caseInfo | 选择框选中的选项内容    | 
| 选项间隔 | 10px |   每个选项之间的间隔  | 
| 字体颜色 | #999999 |  未选中文本的颜色   | 
| 字体大小 | 20px | 未选中文本的大小  | 



#### 未选中
| 配置项 | 默认值  | 功能/备注 |
| :--- | :--- | :--- | 
| 字体颜色 | #ffa84e |  选中文本的颜色   | 
| 字体大小 | 20px | 选中文本的大小  | 

> ## 开发模式

### 参数配置列表

```
{
    'type': 'MultiCheckbox',
    'consist': 'checkbox',
    'orient': 'horizontal',
    'itemGap': '10',
    'iconGap': '5',
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
            'fontSize': '20',
            'backgroundColor': '#fff'
        },
        'checked': {
            'color': '#ffa84e',
            'fontSize': '20'
        }
    }
}
```

### 参数字段说明

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | MultiCheckBox |  | 控件类型——MultiCheckBox选项框，不可修改 |
| consist | String | √ | checkbox | checkbox、radio | 选项种类。checkbox多选；radio单选 |
| itemGap | Number | √ | 10 |  | 选项之间的间隔 |
| iconGap | Number | √ | 5 |  | 选项的勾选框与选项文本框之间的间隔 |
| series | Array\(Object\) | √ |  |  | 选项数据 |
| series\[0\].name | String | √ |  |  | 选项文本内容，可以重复 |
| series\[0\].value | String | √ |  |  | 选项唯一标识，不可重复 |
| checkedValues | Array\(String\) | √ |  |  | 当前为选中状态下的选项标识 |
| itemStyle | Object | √ |  |  | 选项样式 |
| itemStyle.normal | Object | √ |  |  | 选项**未选中**状态样式 |
| itemStyle.normal.color | String | √ | \#999999 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 选项**未选中**状态勾选框与选项文本框内的文本颜色 |
| itemStyle.normal.fontSize | String | √ | 20 | 支持CSS3中font-size的参数值 | 选项**未选中**状态勾选框与选项文本框内的文本大小 |
| itemStyle.normal.backgroundColor | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 选项**未选中**状态勾选框与选项文本框内的背景颜色 |
| itemStyle.checked | Object | √ |  |  | 选项**选中**状态样式 |
| itemStyle.checked.color | String | √ | \#ffa84e | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 选项**选中**状态勾选框与选项文本框内的文本颜色 |
| itemStyle.checked.fontSize | Number | √ | 20 | 支持CSS3中font-size的参数值 | 选项**选中**状态勾选框与选项文本框内的文本大小 |

> 注：
>
> * 选项框尚未绑定数据时，可以对series进行编辑；选项框绑定数据后，series会自动生成相应信息，用户只可以对name值进行修改
> * 用户定义选项框初始化选中状态时可编辑checkedValues，其他情况下chekedValues会根据用户当前操作进行自动修改
>
> * itemStyle.normal、itemStyle.checked中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他选项框样式



