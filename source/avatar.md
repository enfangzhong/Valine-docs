---
title: 头像配置
---
Valine 目前使用的是[Gravatar][1] 作为评论列表头像。

请自行登录或注册[Gravatar][1]，然后修改自己的头像。

评论的时候，留下在[Gravatar][1]注册时所使用的邮箱即可。

感谢`gravatar.cat.net`提供的镜像服务。  

> 如果你修改了头像后发现没有更新，请不要慌张，因为`gravatar.cat.net` 有七天的缓存期，安静的等待吧~


目前`非自定义头像`有以下7种`默认值`可选:  

参数值|表现形式|备注
:-:|:-:|-
空字符串`''`|![Gravatar官方图形](https://gravatar.cat.net/avatar/adb831a7fdd83dd1e2a309ce7591dff8?s=40)|Gravatar官方图形
`mp`|![神秘人(一个灰白头像)](https://gravatar.cat.net/avatar/adb831a7fdd83dd1e2a309ce7591dff8?s=40&d=mm)|神秘人(一个灰白头像)
`identicon`|![抽象几何图形](https://gravatar.cat.net/avatar/adb831a7fdd83dd1e2a309ce7591dff8?s=40&d=identicon)|抽象几何图形
`monsterid`|![小怪物](https://gravatar.cat.net/avatar/adb831a7fdd83dd1e2a309ce7591dff8?s=40&d=monsterid)|小怪物
`wavatar`|![用不同面孔和背景组合生成的头像](https://gravatar.cat.net/avatar/adb831a7fdd83dd1e2a309ce7591dff8?s=40&d=wavatar)|用不同面孔和背景组合生成的头像
`retro`|![八位像素复古头像](https://gravatar.cat.net/avatar/adb831a7fdd83dd1e2a309ce7591dff8?s=40&d=retro)|八位像素复古头像
`robohash`|![机器人](https://gravatar.cat.net/avatar/00000000000000000000000000000000?s=40&d=robohash&f=y)|一种具有不同颜色、面部等的机器人
`hide`|&nbsp;|不显示头像

```js
new Valine({
    ...
    avatar:'' // (''/mp/identicon/monsterid/wavatar/robohash/retro/hide)
});
```

在主题配置文件中搜索valine,找到valine下的属性avater,修改为如下所示：
```
valine:
  avatar: wavatar # gravatar style
```

[1]:http://cn.gravatar.com/
