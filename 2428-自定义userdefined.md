# 选项框\_RadioButton ![](/assets/radiobutton.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'UserDefied',
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

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | UserDefined |  | 控件类型——UserDefined自定义，不可修改 |
| content | String | √ |  |  | 自定义控件代码 |
| series | Array\(Object\) | √ |  |  | 自定义控件中的数据 |
| series.name | String | √ |  |  | 选项文本内容，可以重复 |
| series.value | String | √ |  |  | 选项唯一标识，不可重复 |


