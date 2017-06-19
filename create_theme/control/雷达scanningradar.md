# 雷达\_ScanningRadar ![](/assets/ScanningRadar.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'scanningRadar': {
        'splitLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#0afea4'
            }
        },
        'axisLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#0afea4'
            }
        }
    },
    'series': [
        {
            'type': 'scanningRadar',
            'colors': [
                'white',
                '#10a7ba',
                'white'
            ]
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
        <td> scanningRadar | Object </td>
        <td>雷达底图样式</td>
        <td> </td>
    </tr>
    <tr>
        <td> scanningRadar.splitLine | Object </td>
        <td>雷达底图圆环样式</td>
        <td> </td>
    </tr>
    <tr>
        <td> scanningRadar.splitLine.show | Bool</td>
        <td>是否显示雷达底图圆环</td>
        <td>true</td>
    </tr>
    <tr>
        <td> scanningRadar.splitLine.lineStyle | Object</td>
        <td>雷达底图圆环线样式</td>
        <td><pre>
            {
                'stroke': '#0afea4'
            }
        </pre></td>
    </tr>
    <tr>
        <td>scanningRadar.axisLine | Object </td>
        <td>雷达底图辅助线</td>
        <td> </td>
    </tr>
    <tr>
        <td>scanningRadar.axisLine.show | Bool </td>
        <td>是否显示雷达底图辅助线</td>
        <td>true</td>
    </tr>
    <tr>
        <td>scanningRadar.axisLine.lineStyle | Object </td>
        <td>雷达底图辅助线样式</td>
        <td><pre>
            {
                'stroke': '#0afea4'
            }
        </pre></td>
    </tr>
    <tr>
        <td>series | Array\(Object\) </td>
        <td>雷达扫描片配色样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>series\[0\].type | String </td>
        <td>控件类型——scanningRadar雷达，不可修改 </td>
        <td>true</td>
    </tr>
    <tr>
        <td>series\[0\].colors | String </td>
        <td>雷达扫描片配色组 </td>
        <td><pre>
            [
                'white',
                '#10a7ba',
                'white'
            ]
        </pre></td>
    </tr>
</table>
