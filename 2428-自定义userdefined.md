# 自定义\_UserDefined ![](/assets/UserDefined.png)

---

> ## 编辑模式

## ![](/assets/userdefined01.png)

* 进入代码编辑器，使用VUE.js，编辑完成后**保存返回**主页面单击对勾√按钮，**直接返回**单击×按钮。

## ![](/assets/userdefined02.png)

> ## 开发模式

### 参数配置列表

```
{
    'type': 'UserDefined',
    'content': '<style> @@TE@@    div#UserDefiedapp {  @@TE@@    background-color: green;  @@TE@@    width: 300px;  @@TE@@    height: 50px; @@TE@@    line-height: 50px;  @@TE@@    } @@TE@@</style> @@TE@@<template>  @@TE@@    <div id="UserDefiedapp">{{message}}</div> @@TE@@</template>@@TE@@<script>    @@TE@@    new Vue({@@TE@@        el: "#UserDefiedapp",@@TE@@        data: {@@TE@@                message: "Hello Vue.js! You can use Vue in this control"@@TE@@            }@@TE@@        }) @@TE@@</script>',
    'series': [
        {
            'name': '群众求助',
            'value': 651
        },
        {
            'name': '交通类',
            'value': 594
        },
        {
            'name': '纠纷类',
            'value': 378
        },
        {
            'name': '违法类',
            'value': 219
        },
        {
            'name': '求助类',
            'value': 133
        }
    ]
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
	<td>控件类型——UserDefined自定义，不可修改</td>
	<td>UserDefined</td>
</tr>
<tr>
	<td>content | String</td>
	<td>自定义控件代码</td>
	<td></td>
</tr>
<tr>
	<td>series | Array[Object]</td>
	<td>数据系列配置</td>
	<td></td>
</tr>
<tr>
	<td>series[0].name | String</td>
	<td>数据的文本内容，可以重复</td>
	<td></td>
</tr>
<tr>
	<td>series[0].value | Array[Object]</td>
	<td>数据的唯一标识，不可重复</td>
	<td></td>
</tr>
</table>

> 注：
>
> * @@TE@@为换行转义字符
> * 关于content中的VUE.js代码编辑，建议使用用户配置项，具体操作详见用户配置
> * 自定义控件尚未绑定数据时，可以对series\[0\].data进行编辑；自定义控件绑定数据后，series会自动生成相应信息，用户只可以对name值进行修改


