### ZxwyWebsite/cloudreve
Cloudreve其它架构版本  
整合包请解压到一个文件夹  
已支持架构：s390x，armv7，armv5，armv6，amd64  
已支持系统：Windows，Linux  
CDN加速下载：https://b2eu.zw-cdn.tk/gh/cloudreve/{路径}/{包名}
#### 公告&更新
**\> 2022-02-08**  
【踩坑】  
终于搞明白怎么将前端打包进程序了（...）  
打包前端目录结构应为 assets.zip/assets/build/{前端文件}  

【后端】  
去除更新检测，位置 /bootstrap/app.go  

【前端】  
使用2022-07-12克隆下载的版本，可在设置中切换语言  
删除设置里的 "关于Cloudreve" 选项，位置 /assets/src/component/Setting/UserSetting.js  
删除后台首页的社区文章，位置 /assets/src/component/Admin/Index.js  
使用细滚动条（测试）  

【问题】  
Cloudreve的站点描述显示异常（{siteDes}获取不到）  
是很早以前的Bug了，不信你去官方demo看一下  
暂时可通过手动修改index.html解决  

【公告】  
暂时还是不打算更新3.6系列，因为据论坛反馈还有一些bug，再等一段时间吧...  
感谢 https://github.com/ZxwyWebSite/cloudreve/issues/1 提供思路，在 VBox+Ubuntu22.04 虚拟机上编译成功，到arm平台报错 No such file or directory。。。  
只能用老方法先编译了个armv6版本凑合着用吧，估计同样方法做的s390x版本也用不了  
之前用来编译s390x版本的linuxone机器到期了，等几天重新申请一个就能更新了

**\> 2022-12-28**  
最近cloudreve更新了3.6版本，但由于在修bug会频繁更新，暂不考虑添加，等稳定了再添加  
github直接下载慢可使用cdn：[https://gcore.jsdelivr.net/gh/ZxwyWebSite/cloudreve/](https://gcore.jsdelivr.net/gh/ZxwyWebSite/cloudreve/){包名}  
jsd有文件大小限制，无法下载请使用自建cdn：[https://b2eu.zw-cdn.tk/gh/cloudreve/](https://b2eu.zw-cdn.tk/gh/cloudreve/){包名}
