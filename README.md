# statistics

> 数据统计 js 版 


> 数据格式

```
## 返回值： 0 or 1
## 入参 data 以base64进行加密
eg. 
http://xxxxxxxx/track/?data= base64_encode....
{
    "event":"$web_event",																#web事件
    "properties":{																		#属性
        "$os":"iOS",        															#系统
        "$browser":"Mozilla",															#浏览器
        "$device":"iPhone",																#设备
        "$current_url":"http://localhost:8080/mixpanel",								#当前路径
        "$browser_version":null,														#浏览器版本
        "$screen_height":667,															#屏幕高度
        "$screen_width":375,															#屏幕宽度
        "mp_lib":"web",																	#web使用
        "$lib_version":"2.9.16",														#库版本号
        "distinct_id":"1590697a5f679-0971b331aac6d7-574e6e46-3d10d-1590697a5f743f",		#*****UUID[时间戳+随机+UA+屏幕*宽高+时间戳]
        "$initial_referrer":"$direct",													#*****页面来源，若无值为“$direct”
        "$initial_referring_domain":"$direct",											#*****页面来源域名，若无值为“$direct”
        "$title":"Document",															#当前页面标题
        "$event_type":"pageview",														#事件类型[click,change,submit]默认pageview
        "$ce_version":1,																#ce版本
        "$host":"localhost:8080",														#当前host
        "$pathname":"/mixpanel",														#pathname
        "$elements":[																	#数组：递归到body
            {
                "classes":[																#数组：标签所有样式类
                    ""																	
                ],
                "tag_name":"div",														#标签名
                "attr__style":"position:fixed;left:0;bottom:0;",						#行内样式
                "attr__class":"suc first-page",						
                "nth_child":2,															# 第几个孩子
                "nth_of_type":1															# 同一标签的第一个
            },
            {
                "classes":[
                    ""
                ],
                "tag_name":"body",
                "nth_child":2,
                "nth_of_type":1
            }
        ],
        "$el_text":"",																#标签文本
        "token":"9fc8c3575b8b5125aaee8e77f5f71cb1",										#token--为唯一标识，与之前userid类似
        "$__c":0																		#**添加dom事件次数add_dom_event_counting
    }
}
```