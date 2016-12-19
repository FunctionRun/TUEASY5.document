# 菜单\_TreeMenu

---

> ## 开发模式

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
    'selectedValue': '北京市',
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

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/描述 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | treeMenu |  | 控件类型——TreeMenu菜单，不可修改 |
| series | Array\(Object\) | √ |  |  | 菜单数据项 |
| series | Bool | √ | false |  | 是否播放音频 |
| videoSrc | String | √ |  |  | 视频播放地址 |
| videoStyle | Object |  |  |  | 视频的样式 |

> 注：
>
> * videoStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他视频样式



