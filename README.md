
# 根据神图壁纸小程序 整理所需要的接口，字段 (非全部功能 ，整理了一些重要的功能)

  第一个版本先实现基本功能 

## 1.首页前端界面 就一个搜索框 输入口令 搜索壁纸

接口根据前端传入口令 返回壁纸列表 

``` JSON
{
    "images":[
        "http://xxxxx.png",
        "http://xxxxx.png"
    ]
}
```
上面返回的是缩略图的地址 可以在缩略图的基础上加上符号变成 高清图的地址 

例如 缩略图地址是 http://xxxxx.png 那么高清图地址就是 http://xxxxx_hd.png

因为高清图可能非常大 图片需要两种分辨率 一种是缩略图 一种是高清图 列表显示缩略图(分辨率低的图片) 点击图片列表的一个项目 打开高清图页面


## 2.小程序集成抖音广告组件
在用户点击下载的时候弹出观看广告 观看后允许下载


## 3.用户登入接口 客户端获取抖音登入的code后
传给服务端 用户第一次登入创建用户然后返回用户信息，否则直接返回用户信息 
``` JSON
{
    "id" : 1,
    "isCreator" : true //是否是创作者
}
```
目前考虑发布作品放在小程序 这样就不用写一个管理后台 

如果是创作者需要有一个上传图片的入口 点击打开上传页面 然后用户输入口令 (需要一个检查口令是否被使用的接口 如果口令已经被使用提醒创作者换口令) 上传图片 点击提交给服务端








