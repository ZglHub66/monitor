### 浏览器设备模块
#### 使用
>直接使用(引入js文件)
~~~
var info= DeviceInfo.getDeviceInfo({
  domain:'xxx',// 用于生成浏览器指纹 不传或为空时默认为:window.location.host
  info:['deviceType','userAgent','UUID']//需要获取的浏览器信息数组 不传默认全部获取 当前代码演示:`获取设备类型`,`浏览器信息`,`唯一标识`
 });
 //var info= DeviceInfo.getDeviceInfo();//默认获取全部信息
<!-- 通过info接收需要的浏览器信息进行后续处理  -->
~~~

> ##### INFO 配置项
|             Name             |  说明  | 属性值                                                         |
| :--------------------------: | :----: | ------------------------------------------------------------ |
| deviceType | 设备类型 | `PC`,`Mobile`,`Tablet` |
| OS | 系统或平台 | `Windows`, `Linux`, `Mac OS`, `Android`, `HarmonyOS`, `Ubuntu`, `FreeBSD`, `Debian`, `Windows Phone`, `BlackBerry`, `MeeGo`, `Symbian`, `iOS`, `Chrome OS`, `WebOS` |
| OSVersion | 操作系统版本 | ... |
| screenHeight | 屏幕高 | ... |
| screenWidth | 屏幕宽 | ... |
| language | 当前使用的语言-国家 | ... |
| netWork | 联网类型 | ... |
| orientation | 横竖屏 | ... |
| browserInfo | 浏览器信息 | ... |
| fingerprint | 浏览器指纹 | ... |
| userAgent | 浏览器信息 包含 appCodeName,appName,appVersion,language,platform 等 | ... |
| UUID | 生成通用唯一标识 | ... |
| canvas | 是否支持canvas | `true`,`false` |
| webgl | 是否支持webgl | `true`,`false` |
