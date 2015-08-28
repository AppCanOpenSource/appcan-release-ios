# appcan-release-ios
### 2015/8/28版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_150828_01      更新内容：
   * app进入后台时 不再会调用插件的clean方法   * 解决appkey获取不到的问题
   * 修复关闭侧边栏窗口时的黑屏问题
   * 优化finishWidget方法
   * 解决appkey获取不到的问题
   * 增加uexWindow.getSlidingWindowState()接口及其回调


####iOS插件：
 1. 插件名称及版本号：uexGaodeMap-3.0.4
       更新内容：
    * 添加自定义按钮功能
    * 地理编码和反地理编码的回调添加参数,方便用户区分
 2. 插件名称及版本号：uexActionSheet-3.0.6
       更新内容：修复textNColor属性失效的bug
 3. 插件名称及版本号：uexJPush-3.0.3
       更新内容：修改推送的extras为字典格式   
***

### 2015/8/25版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexJPush-3.0.2
       更新内容：
    * 添加对config.xml配置的支持
    * onReceiveNotificationOpen添加延时
***
### 2015/8/24版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_150824_01      更新内容：
   * 修正盒子用户不能正常解密的bug   * 修正全包加密情况下不能打开http/https网页的BUG   * MBProgressHUD 第三方库更新
***

### 2015/8/21版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexUploaderMgr-3.0.7      更新内容：修改了请求头的验证
 2. 插件名称及版本号：uexDownloaderMgr-3.0.5      更新内容：修改了请求头的验证
    
 3. 插件名称及版本号：uexXmlHttpMgr-3.0.10      更新内容：修改获取appkey的方法
 4. 插件名称及版本号：uexEasemob-3.0.13      更新内容：
    * 修复sendLocation接口 不能正确解析经度的bug	* 修复updatePushOptions 有时会失效的bug 
 ***

### 2015/8/14版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexSearchBarView-3.0.0      更新内容：新增
 ***
### 2015/8/7版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexGaodeMap-3.0.3      更新内容：
    
	* 修复使用自定义气泡时自定义标注图标失效的问题
 	* 修复覆盖物设置透明色会失效的bug
 	* 修复getCurrentLocation不敏感的bug
 	* 修复clear接口可能会导致闪退的bug
 ***

### 2015/7/31版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexImageBrowser-3.0.18      更新内容：uexImageBrowser.pick新增可选参数，可以返回无损画质图片
 2. 插件名称及版本号：uexFileMgr-3.0.11      更新内容：新增cbWiriteFile方法
 3. 插件名称及版本号：uexChatKeyboard-3.0.4
       更新内容：新增API：获取键盘高度
 4. 插件名称及版本号：uexBluetoothLE-3.0.0
 	更新内容：新增
 5. 插件名称及版本号：uexEasemob-3.0.12
 	更新内容：
 	* 新增API:getRecentChatters，onMessageSent
 	* 添加创建群回调onGroupCreated

***
### 2015/7/24版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexWeiXin-3.0.16      更新内容：图文分享添加可选参数title
 2. 插件名称及版本号：uexGaodeMap-3.0.2      更新内容：
	* 新增removeMarkersOverlays、removeOverlays、setScaleVisible接口    * 现在iOS也支持onMapClickListener 点击地图的监听方法了    * 现在iOS也支持onMapLongClickListener 长按地图的监听方法了    * 新增离线地图相关方法，优化添加标注接口使其支持自定义气泡    * 支持config.xml配置appKey(配合打包服务器公测）    用户需要将如下字段中的XXX替换为自己申请的key，然后添加至config.xml中：
    	```
		<config desc="uexGaode" type="KEY" > 	    	<param platform="iOS" name="$uexGaodeMap_APIKey$"  value="XXX"/>      	</config>
	
		```
   
***

### 2015/7/17版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_150717_02      更新内容：移除对本地通知的相关处理

####iOS插件：
 1. 插件名称及版本号：uexLocalNotification-3.0.3      更新内容：添加对接收到本地通知的处理方法
 2. 插件名称及版本号：uexIndexBar-3.0.6      更新内容：    * 索引表可以设置是否随网页滑动    * 修改多次open之后不能成功close的问题
***

### 2015/7/10版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexLocation-3.0.19      更新内容：修复点击点击返回应用闪退的问题
 2. 插件名称及版本号：uexZip-3.0.2         更新内容：解决压缩和解压缩大文件会卡屏的问题
 3. 插件名称及版本号：uexFileMgr-3.0.10
       更新内容：解决多选文件打开浏览器空白问题
 4. 插件名称及版本号：uexXmlHttpMgr-3.0.8
       更新内容：新增API  clearCookie
     5. 插件名称及版本号：uexClipboard-3.0.2
       更新内容：修复被复制的文本包含换行符会导致插件异常的bug
 6. 插件名称及版本号：uexJPush-3.0.1       更新内容：
 	* init接口废弃，现在插件会在App启动时自动初始化（与Android保持一致） 	* 支持onReceiveNotificationOpen接口 用户在点击Apns通知打开App时，会触发此回调     7. 插件名称及版本号：uexEasemob-3.0.10      更新内容：
    * 现在能够传正确的boolean值true、false给网页，而不是”true” 、”false”	* EMGroup结构回调添加groupName、groupDescription属性，原groupSubject属性废弃 8. 插件名称及版本号：uexChart-3.0.0      更新内容：新增
    
 9. 插件名称及版本号：uexAreaPickerView-3.0.3       更新内容：返回数据添加空格便于分割    
***
### 2015/7/3版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_150706_02      更新内容： 
 1. 新增isAppInstalled及回调；新增监听onWindowAppear、onWindowDisappear 2. 新增reload,reloadWidgetByAppId
 3. 修改widget未初始化就使用的问题

####iOS插件：
 1. 插件名称及版本号：uexWeiXin-3.0.15      更新内容：cbStartPay回调结构修正
***    
### 2015/6/25版本更新记录

####iOS插件：
 1. 插件名称及版本号：uexQQ-3.0.6      更新内容：cbLogin回调结构修正
 2. 插件名称及版本号：uexSina-3.0.5      更新内容：注册回调方法名统一修改为uexSina.cbRegisterApp
 3. 插件名称及版本号：uexFileMgr-3.0.9
       更新内容：新增方法uexFileMgr.renameFile 重命名文件及其回调uexFileMgr.cbRenameFile
 4. 插件名称及版本号：uexLocalNotification-3.0.2      更新内容：修复iOS8.0+系统上可能不能正常发送通知的bug
     5. 插件名称及版本号：uexAreaPickerView-3.0.2      更新内容：新增
 6. 插件名称及版本号：uexCalendarView-3.0.0      更新内容：新增
     7. 插件名称及版本号：uexChatKeyboard-3.0.3      更新内容：新增
 8. 插件名称及版本号：uexInputTextFieldView-3.0.3      更新内容：新增
 9. 插件名称及版本号：uexLoadingView-3.0.3      更新内容：新增
 10. 插件名称及版本号：uexIndexBar-3.0.5
       更新内容：索引文字支持配置颜色和内容
 11. 插件名称及版本号：uexQQ-3.0.8.zip
       更新内容：不再支持分享至QQ好友的所有相关接口中的cflag可选参数
***
### 2015/6/19版本更新记录

####iOS引擎：            版本号：ios_Engine_3.1_150619_01      更新内容： 
 1. setMultilPopoverFlippingEnbaled与安卓统一效果
  2. addSubViewToScrollView 修复手势被网页错误拦截的问题 	          ####iOS插件：
 1. 插件名称及版本号：uexEasemob-3.0.9      更新内容： 
    * 添加getTotalUnreadMsgCount接口
    * 获取全部公开群改成分页获取

***
### 2015/6/12版本更新记录

####iOS引擎：
  
  版本号：ios_Engine_3.1_150612_01    更新内容：修复了在popover页面中不能正确执行openMultiPopover的bug.

                       ####iOS插件：          1. 插件名称及版本号：uexAreaPickerView --3.0.2
	 	更新内容：修复了插件会因失去焦点而被错误关闭的bug.
***

### 2015/6/5版本更新记录
####iOS插件：

1.	插件名称及版本号：uexWeiXin-3.0.14
	
	更新内容：uexWeiXin插件，支付sdk升级。
	

	

***
### 2015/5/29版本更新记录
####iOS插件：

1.	插件名称及版本号：uexEasemob-3.0.8
	
	更新内容：
	
	* 新增 发送视频消息 和 发送已读回执 的接口;	
	* 发送的消息，新增ext和length属性；
	* 修复bugs.
	
2. 插件名称及版本号：uexJPush-3.0.0

 	更新内容：新增极光推送插件
 	
3. 插件名称及版本号：uexScrollPicture-3.0.0
	
	更新内容：新增轮播图插件
	
	
	

***
### 2015/5/20版本更新记录

####iOS引擎：
  
  版本号：ios_Engine_3.1_150520_01    更新内容：

1. 新增uexWindow.setMultilPopoverFlippingEnbaled()方法；2. 添加webview嵌view方法（非API接口，供自定义插件调用）；3. 新增onPopoverLoadFinishInRootWnd(name,url)监听方法；4. 修复setBounce会导致滚动条消失的bug；                         5. 添加reachabilityWithHostname方法。

                       ####iOS插件：          1. 插件名称及版本号：uexAliPay-3.0.8
 	更新内容：支付宝插件升级  2. 插件名称及版本号：uexXmlHttpMgr-3.0.7
 	更新内容：onData回调函数参数修改 3. 插件名称及版本号：uexDownloaderMgr-3.0.3
 	更新内容：修复不支持HTTPS问题 4. 插件名称及版本号：uexUploaderMgr-3.0.6
 	更新内容：修复不支持HTTPS问题 5. 插件名称及版本号：uexAudio-3.0.10
 	更新内容：更新MP3编码lame库；提高录音功能输出的MP3文件的采样率；修复生成的录音mp3文件不能通过http方式播放的bug。 6. 插件名称及版本号：uexGaodeMap-3.0.0
 	更新内容：新增高德地图插件
