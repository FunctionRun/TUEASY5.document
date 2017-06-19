# 图片\_Picture ![](/assets/Picture-icon.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Image',
    'selected': false,
    'normal': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px',
            'marginLeft': 0,
            'marginTop': 0
        }
    },
    'mouse': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px',
            'marginLeft': 0,
            'marginTop': 0
        }
    },
    'emphasis': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px'
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
        <td>type | String </td>
        <td> 控件类型——Image图片，不可修改 </td>
        <td>Image </td>
    </tr>
    <tr>
        <td>selected | Bool </td>
        <td> 图片是否为选中状态 </td>
        <td> false </td>
    </tr>
    <tr>
        <td>normal | Object </td>
        <td>图片**未选中**状态样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>normal.src | String </td>
        <td>图片**未选中**状态资源地址 </td>
        <td> </td>
    </tr>
    <tr>
        <td>normal.text | String </td>
        <td>图片**未选中**状态的文本内容 </td>
        <td> </td>
    <tr>
        <td>normal.imageStyle | Object </td>
        <td>图片**未选中**状态图片样式 </td>
        <td><pre>
            {
                'borderRadius': '1px',
                'opacity': '1'
            }
        </pre></td>
    </tr>
    <tr>
        <td>normal.textStyle | Object</td>
        <td>图片**未选中**状态的文本样式 </td>
        <td><pre>
            {
                'color': '#ccc',
                'fontSize': '14px',
                'marginLeft': 0,
                'marginTop': 0
            }
        </pre></td>
    </tr>
    <tr>
        <td> mouse | Object  </td>
        <td>图片**鼠标悬浮**状态样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td> mouse.src | String </td>
        <td>图片**鼠标悬浮**状态资源地址 </td>
        <td> </td>
    </tr>
    <tr>
        <td> mouse.text | String </td>
        <td>图片**鼠标悬浮**状态的文本内容 </td>
        <td> </td>
    <tr>
        <td> mouse.imageStyle | Object </td>
        <td>图片**鼠标悬浮**状态图片样式 </td>
        <td><pre>
            {
                'borderRadius': '1px',
                'opacity': '1'
            }
        </pre></td>
    </tr>
    <tr>
        <td> mouse.textStyle </td>
        <td>图片**鼠标悬浮**状态的文本样式 </td>
        <td><pre>
            {
                'color': '#ccc',
                'fontSize': '14px',
                'marginLeft': 0,
                'marginTop': 0
            }
        </pre></td>
    </tr>
    <tr>
        <td>emphasis | Object </td>
        <td>图片**选中**状态样式 </td>
        <td> </td>
    </tr>
    <tr>
        <td>emphasis.src | String </td>
        <td>图片**选中**状态资源地址 </td>
        <td> </td>
    </tr>
    <tr>
        <td>emphasis.text | String </td>
        <td>图片**选中**状态的文本内容 </td>
        <td> </td>
    </tr>
    <tr>
        <td>emphasis.imageStyle | Object </td>
        <td>图片**选中**状态图片样式 </td>
        <td><pre>
            {
                'borderRadius': '1px',
                'opacity': '1'
            }
        </pre></td>
    </tr>
    <tr>
        <td>emphasis.textStyle</td>
        <td>图片**选中**状态的文本样式 </td>
        <td><pre>
            {
                'color': '#ccc',
                'fontSize': '14px'
            }
        </pre></td>
    </tr>
</table>

> 注：
>
> * normal.imageStyle和normal.textStyle、mouse.imageStyle和mouse.textStyle、emphasis.imageStyle和emphasis.textStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他图片样式



