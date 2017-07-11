# 菜单\_TreeMenu ![](/assets/TreeMenu.png)

---

![](/assets/TreeMenu01.png)
![](/assets/TreeMenu03.png)
![](/assets/TreeMenu04.png)
![](/assets/TreeMenu05.png)

## 开发模式

![](/assets/TreeMenu02.png)

### 参数配置列表

```
{
    'type': 'treeMenu',
    'series': [
        {
            'name': '北京市',
            'value': 'beijing',
            'childrens': [
                {
                    'name': '朝阳区',
                    'value': 'chaoyangqu',
                    'childrens': [
                        {
                            'name': '朝阳公园',
                            'value': 'chaoyang park'
                        },
                        {
                            'name': '三里屯',
                            'value': 'sanlitun'
                        }
                    ]
                },
                {
                    'name': '海淀区',
                    'value': 'haidianqu'
                }
            ]
        },
        {
            'name': '上海市',
            'value': 'shanghai',
            'childrens': [
                {
                    'name': '徐汇区',
                    'value': 'xuhuiqu'
                },
                {
                    'name': '松江区',
                    'value': 'songjiangqu'
                },
                {
                    'name': '嘉定区',
                    'value': 'jiadingqu'
                }
            ]
        },
        {
            'name': '重庆市',
            'value': 'chongqing',
            'childrens': [
                {
                    'name': '渝北区',
                    'value': 'yubeiqu'
                },
                {
                    'name': '渝中区',
                    'value': 'yuzhongqu'
                },
                {
                    'name': '北碚区',
                    'value': 'beibeiqu'
                }
            ]
        }
    ],
    'titleName': '北京市',
    'SubTreeGap': 30,
    'itemStyle': {
        'primaryStyle': {
            'height': '40px',
            'fontFamily': '微软雅黑',
            'fontSize': '14px',
            'color': '#fff',
            'display': 'inline-block',
            'backgroundColor': 'rgb(102, 118, 136)',
            'lineHeight': '40px'
        },
        'primaryArrowStyle': {
            'fontSize': '18px',
            'color': 'rgb(255, 255, 255)'
        },
        'menuStyle': {
            'normal': {
                'fontSize': '14px',
                'color': '#fff',
                'backgroundColor': 'rgb(102, 118, 136)',
                'fontFamily': '微软雅黑',
                'lineHeight': '30px'
            },
            'emphasis': {
                'color': '#1C243B',
                'backgroundColor': 'rgb(239, 241, 243)'
            }
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
        <td> type | String</td>
        <td>控件类型——TreeMenu菜单，不可修改 </td>
        <td>treeMenu</td>
    </tr>
    <tr>
        <td> series | Array\(Object\)</td>
        <td>菜单数据项，每一个数组元素\(Object\)代表一个一级项 </td>
        <td> </td>
    </tr>
    <tr>
        <td> series\[0\].name | String</td>
        <td>菜单项文本内容，可以重复 </td>
        <td> </td>
    </tr>
    <tr>
        <td> series\[0\].value | String</td>
        <td>菜单项唯一标识 </td>
        <td> </td>
    </tr>
    <tr>
        <td> series\[0\].children | Object</td>
        <td>该级菜单项下的子菜单项，结构同一级项一样 </td>
        <td> </td>
    </tr>
    <tr>
        <td> titleName | String </td>
        <td>初始化菜单时的默认菜单项文本内容。仅用于初始化显示，未选中当前任何菜单项 </td>
        <td> </td>
    </tr>
    <tr>
        <td> SubTreeGap | String </td>
        <td>子菜单距离父级菜单向右缩进的距离 </td>
        <td>30px</td>
    </tr>
    <tr>
        <td> itemStyle | Object </td>
        <td>菜单项的样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td> itemStyle.primaryStyle | Object </td>
        <td>菜单项显示栏的样式 </td>
        <td><pre>
{
    'height': '40px',
    'fontFamily': '微软雅黑',
    'fontSize': '14px',
    'color': '#fff',
    'display': 'inline-block',
    'backgroundColor': 'rgb(102, 118, 136)',
    'lineHeight': '40px' 
}
    </pre></td>
    </tr>
    <tr>
        <td> itemStyle.primaryArrowStyle| Object </td>
        <td>菜单项显示栏的三角标样式  </td>
        <td><pre>
{
    'fontSize': '18px',
    'color': 'rgb(255, 255, 255)'
}
        </pre></td>
    </tr>
    <tr>
        <td>itemStyle.menuStyle | Object </td>
        <td>菜单项下拉菜单的样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>itemStyle.menuStyle.normal | Object  </td>
        <td>下拉菜单**未选中**状态样式 </td>
        <td><pre>
{
    'fontSize': '14px',
    'color': '#fff',
    'backgroundColor': 'rgb(102, 118, 136)',
    'fontFamily': '微软雅黑',
    'lineHeight': '30px'
}
        </pre></td>
    </tr>
    <tr>
        <td>itemStyle.menuStyle.emphasis | Object  </td>
        <td>下拉菜单**选中**状态样式  </td>
        <td><pre>
{
    'color': '#1C243B',
    'backgroundColor': 'rgb(239, 241, 243)'
}
        </pre></td>
    </tr>
</table>

> 注：
>
> * 菜单尚未绑定数据时，series中的children可以无限嵌套，建议一般三级菜单最号；绑定数据后series会自动生成，用户可根据自己需求手动修该文本内容
> * itemStyle.primaryStyle、itemStyle.primaryArrowStyle、itemStyle.menuStyle.normal和itemStyle.menuStyle.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他菜单样式



