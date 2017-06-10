# 选项框\_MultiCheckBox ![](/assets/MultiCheckBox.png)

---

> ## 编辑模式

用户可以通过下方编辑模式面板实现对多选项框的显示内容和样式的快速编辑。![](/assets/MultiCheckBoxUser.jpg)注：初始化选中内容填写的是与显示内容相对应的标识字段。


> ## 开发模式

### 参数配置列表

```
{
    'type': 'MultiCheckbox',
    'consist': 'checkbox',
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

<table border="1">
<tr>
	<th width="15%">配置项</th>
	<th width="30%">功能/描述</th>
	<th>可选参数</th>
</tr>
<tr>
	<td>type | String</td>
	<td>控件类型——MultiCheckBox选项框，不可修改</td>
	<td>MultiCheckBox</td>
</tr>
<tr>
	<td>consist | String</td>
	<td>选项框类型，checkbox为多选；radio为单选</td>
	<td>checkbox、radio</td>
</tr>
<tr>
	<td>orient | String</td>
	<td>选项框对其方式，horizontal为水平对齐；vertical为垂直对齐</td>
	<td>horizontal、vertical</td>
</tr>
<tr>
	<td>itemGap | String</td>
	<td>选项框中选项之间的间距</td>
	<td></td>
</tr>
<tr>
	<td>iconGap | String</td>
	<td>选项框中选项的勾选框与选项文本框之间的间隔</td>
	<td></td>
</tr>
<tr>
	<td>series | Array[Object]</td>
	<td>数据系列配置</td>
	<td></td>
</tr>
<tr>
	<td>series[0].name | String</td>
	<td>选项数据显示时的文本内容，可以重复</td>
	<td></td>
</tr>
<tr>
	<td>series[0].value | Array[Object]</td>
	<td>选项数据的唯一标识，不可重复</td>
	<td></td>
</tr>
<tr>
	<td>checkedValues | Array[String]</td>
	<td>初始化选项框时选中状态的选项标识</td>
	<td></td>
</tr>
<tr>
	<td>itemStyle | Object</td>
	<td>选项框中选项样式，有normal和checked两个属性</td>
	<td></td>
</tr>
<tr>
	<td>itemStyle.normal | Object</td>
	<td>选项框中选项<b>未选中</b>状态的样式</td>
	<td><pre> {
	//文本颜色，支持CSS3中颜色的参数值
	'color': '#999999',
	//文本大小，支持CSS3中font-size的参数值
	'fontSize': '20px',
	//背景颜色，支持CSS3中颜色的参数值
	'backgroundColor': '#fff'
  }</pre></td>
</tr>
<tr>
	<td>itemStyle.checked | Object</td>
	<td>选项框中选项<b>选中</b>状态的样式</td>
	<td><pre> {
	'color': '#ffa94e',
	'fontSize': '20px',
	'backgroundColor': '#fff'
  }</pre></td>
</tr>
</table>

> 注：
>
> * 选项框尚未绑定数据时，可以对series进行编辑；选项框绑定数据后，series会自动生成相应信息，用户只可以对name值进行修改
> * 用户定义选项框初始化选中状态时可编辑checkedValues，其他情况下chekedValues会根据用户当前操作进行自动修改
>
> * itemStyle.normal、itemStyle.checked中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他选项框样式



