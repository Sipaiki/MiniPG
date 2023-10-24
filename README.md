
# 参考类似壁纸小程序 整理所需要的接口，字段 (非全部功能 ，整理了一些重要的功能)

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

## 3.管理后台 管理后台用来给用户创建主页 主页有主页名称 头像 页面口令 在主页下可以上传图片 一个用户可以创建多个主页
前端需要部署一个管理后台项目 后端需要一个创建主页接口 检查口令是否可用接口 上传文件接口 

## 4. 目前可不做 用户登入接口 
客户端获取抖音登入的code后 可以换取 openid、unionid, openid 是用户在当前小程序的 ID，unionid 是用户在小程序平台的唯一标识符 把unionid
传给服务端 用户第一次登入创建用户然后返回用户信息，否则直接返回用户信息 用户信息 如下JSON
``` JSON
{
    "id" : 1,
    "isCreator" : true //是否是创作者
}
```






