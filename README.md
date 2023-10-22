
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

## 2.小程序集成免费的三方全埋点 通过收集 小程序的访问量 搜索点击量 下载点击量 快速测试这个项目



