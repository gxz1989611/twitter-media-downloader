# twitter-media-downloader
用于提取推特页面中包含的媒体数据（支持图片, 视频, 动图）的脚本  
<br/>

支持输入如下三种格式的链接:
1. https://<span></span>twitter.com/\*\*\*/status/\*\*\* (推文)  
2. https://<span></span>t.co/****** (短链, 部分短链会跳转至非推文页面, 脚本会自动跳过)  
3. https://<span></span>twitter.com/\*\*\* (推主主页, \*\*\*为推主id, 用于批量爬取)  
<br/>

PS:    
1. 获取到的媒体文件自动下载到路径下的twitter_media_download文件夹  
2. 已知单条推文仅可能出现4张以内的图片或1个动图/视频
3. 默认使用系统代理，无需配置 (仅win平台, 其余平台请手动设置)
4. 爬取视频文件时, 会自动选择最高分辨率下载
5. 若提取出现任何问题，请反馈log文件  

# TODO (待实现需求)  
1. ~~支持cmd传参调用~~ (完成)
2. ~~支持爬取视频/动图文件~~ (完成)
3. ~~支持批量爬取推主所有媒体~~ (完成)
4. ~~下载进度显示~~ (完成)
5. 支持linux平台
6. 支持手动设置UA和代理
7. 支持设置cookie用于爬取锁推
8. 完善程序错误log导出
9. 批量爬取时输出进度记录, 并在程序异常退出重启后导入进度继续下载
10. ~~在文件名前添加推文id, 方便定位推文~~ (完成)

<img src="https://pic.rmb.bdstatic.com/bjh/e7bb8983c155712b6175e99f9f66ff35.png">
