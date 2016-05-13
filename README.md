# appcan-release-ios
### 2016/05/13版本更新记录
####iOS插件：

1. 版本号：uexAliPay-3.0.9	

   更新内容：
   * 更新支付宝SDK到15.0.6 
   * 优化3.3引擎下传错误的参数类型可能会造成闪退的问题2. 版本号：uexEasemob-3.0.23	
   更新内容：优化删除EaseUIResource.bundle内会引起上架失败的info.plist；3. 版本号：uexQQ-3.0.14	
   更新内容：修改回调逻辑,解决presentWindow收不到回调的问题4. 版本号：uexScanner-3.1.7	
   更新内容：优化为ios7.0以上调用系统库扫描5. 版本号：uexJPush-3.0.8	
   更新内容：更新JPush SDK到2.1.6 6. 版本号：uexScrawl-3.0.1	
   更新内容：优化点击保存按钮无法关闭窗口的问题，与android保持一致。
***
### 2016/05/06版本更新记录
####iOS引擎：
 版本号：ios_Engine_3.3_160506_01 更新内容：
* openMultiPopover对JS SDK做兼容性处理;* 修复当uexWidget.onLoadByOtherApp、uexWidget.onSuspend、uexWidget.onEnterBackground、uexWidget.onResume、uexWidget.onEnterForeground、window.uexStart这几个接口未定义时可能会产生JS警告的问题
***
### 2016/05/05版本更新记录
####iOS引擎：
 版本号：ios_Engine_3.3_160504_01 更新内容：
新增：                 
                                            * uexWindow.prompt添加hint参数                                                      * 新增uexWindow.openPresentWindow接口* 新增uexWindow.publishChannelNotificationForJson接口* 新增uexWindow.disturbLongPressGesture接口  * 引擎工具库添加若干新方法,为原生插件开发者提供便利                                                                                           * 引擎工具库头文件添加详细注释,为原生插件开发者提供便利 优化：
* 优化setMultiPopoverFrame只能改变multiPopover的frame而不能改变其中的网页的frame的问题* 优化setMultiPopoverFlippingEnabled的参数问题，和文档保持一致* 优化前端已经URLEncode过的URL在引擎中会被再次URLEncode的问题* 优化上拉加载view不显示的问题* openPopover现在会先展示UI再加载网页   * 优化uexWindow.onPopoverLoadFinishInRootWnd不是指向最终跳转的URL的问题  * 优化引擎部分接口当传入不正确的参数时会导致闪退的问题

####iOS插件：
1. 版本号：uex3DTouch-3.0.2	
   更新内容：修复可能会与其他包含3DTouch功能的插件冲突的问题						2. 版本号：uexBaiduMap-3.1.17	
   更新内容：修复removeMakersOverlay接口传不当参数会闪退的问题							3. 版本号：uexCamera360-3.0.0		
   更新内容：新增uexCamera360插件						4. 版本号：uexDevice-3.0.9
   更新内容：修改获取设备型号的方式，添加设备型号							5. 版本号：uexImage-3.0.10	
   更新内容：修复在4/4s机型上裁剪接口闪退的问题							6. 版本号：uexInAppPurchase-3.0.3
   更新内容：更新方法
   						7. 版本号：uexLocation-3.0.26	
   更新内容：新增坐标系转换接口,支持wgs84,gcj02,bd09格式相互转换						8. 版本号：uexVideo-3.0.6	
   更新内容：现在在强制全屏模式下,一定会显示关闭按钮

9. 版本号：uexWheelPickView-3.0.1	
   更新内容：新增默认值选项	
10. 版本号：uexKeyChain-3.0.2 
   更新内容：添加接口getDeviceUniqueIdentifier	

11. 版本号：uexCamera-3.0.8	

    更新内容：cbOpenViewCamera回调方法,返回的JSON中增加字段label,替换之前的location										12. 版本号：uexContact-3.0.10	
    更新内容：
    * 新增search,modifyWithId,deleteWithId接口以及cbSearch,cbModifyWithId,cbDeleteWithId回调 
    * 修复cbSearch回调与安卓不一致,参数命名不一致的问题										13. 版本号：uexEasemob-3.0.22	
    更新内容：
    * 升级环信SDK至3.1.2  
    * 添加客服功能 
    * group新增黑名单							14. 版本号：uexFileMgr-3.0.25	
    更新内容：添加base64支持	   ***
### 2016/04/23版本更新记录
####iOS插件：
1. 版本号：uexFileMgr-3.0.24

   更新内容：	
   * 新增bundle方式引用资源，优化IDE插件不显示图标 
   * 优化getFileSizeByPath接口							2. 版本号：uexEasemob-3.0.20	
   更新内容：	优化加入公开群有时会无响应的问题							3. 版本号：uexControl-3.0.16	
   更新内容：	优化对3.3引擎下非string参数造成闪退的情况进行了处理							4. 版本号：uexLoadingView-3.0.6	
   更新内容：	新增IDE支持		
   					5. 版本号：uexAudio-3.0.18	
   更新内容：
   * 优化无法识别播放无后缀文件  
   * 优化播放amr格式时无回调							6. 版本号：uexCamera-3.0.7	
   更新内容：创建bundle存储资源文件，适配国际化							7. 版本号：uexWheelPickView-3.0.0	
   更新内容：新增uexWheelPickView插件
***
### 2016/04/15版本更新记录
####iOS插件：
1. 版本号：uexChatKeyboard-3.0.24	
 
   更新内容：* 修改键盘“+”号切换键盘异常，修改发送按钮自定义（按钮背景色、高亮颜色、文字、字体大小、字体颜色）* 修改发送消息不能显示到最底部、修改录音从0开始	
   						2. 版本号：uexInputTextFieldView-3.0.8	
   更新内容：修改发送按钮自定义（按钮背景色、高亮颜色、文字、字体大小、字体颜色）							3. 版本号：uexInAppPurchase-3.0.2	
   更新内容：优化内购插件		
   					4. 版本号：uexXunfei-3.0.1	
   更新内容：新增uexXunfei插件	
 ***  
### 2016/03/26版本更新记录
####iOS引擎：
 版本号：ios_Engine_3.3_160325_01 更新内容：
 * 优化引擎支持的最低系统版本为7.0 * 优化引擎中插件调用部分代码用JavaScriptCore进行了重构(for 插件开发者)优化支持插件的同步调用，允许插件直接返回值给前端优化插件接收到的参数会正确的反映其数值类型，而不全是NSString优化可以实现独立于UIWebView的JS上下文,从而可以在后台运行JavaScript。优化以下引擎方法现在可以同步返回结果uexWindow.getUrlQueryuexWindow.getStateuexWidgetOne.getPlatform新增如下接口,具体说明详见引擎文档uexWindow.getWidthuexWindow.getHeightuexWindow.putLocalDatauexWindow.getLocalData	
 
####iOS插件：
1. 版本号：uexVideo-3.0.5	
 
   更新内容：
   * 优化了视频录制的接口——   * 支持控制录制时间;   * 支持控制录制分辨率;   * 支持控制录制视频质量;   * 优化了视频播放接口——   * 性能优化:采用全新的API去播放视频,优化了视频的加载速度,降低了CPU占用;   * 界面优化: UI美化;支持各种常用手势去控制播放;网络视频拥有预加载条提示;   * 支持小窗播放，支持小窗跟随网页滑动;   * 对全屏播放的细节做了处理:现在全屏模式下播放器强制横屏，并且不会随手机设置而自动旋转;   * 更多的可选参数去定制播放器界面;   * 为播放状态和播放器被关闭增加了监听;	
   2. 版本号：uexScrawl-3.0.0	
   更新内容：新增涂鸦功能插件	
   3. 版本号：uexGaodeNavi-3.0.0 	
   更新内容：新增高德导航插件	
   4. 版本号：uexQcloudAV-3.0.0	
   更新内容：新增腾讯云视频直播插件	
   5. 版本号：uexNIM-3.0.0	
   更新内容：新增网易云信插件	
   6. 版本号：uexBackground-3.0.0	
   更新内容：新增实现后台运行JS的功能（对应uexlocation插件更新了，配合测试）	7. 版本号：uexLocation-3.0.24	
   更新内容：新功能，优化定位权限,支持后台定位
  ***

### 2016/03/16版本更新记录
####iOS插件：
1.版本号：uexLoadingView-3.0.5

更新内容：优化openCircleLoading在ios7上背景不透明

2.版本号：uexScanner-3.1.6

更新内容：新增charset字段设置编码


3.版本号：uexImage-3.0.9

更新内容：优化pick接口选取拍摄的照片时方向可能不正确

4.版本号：uexPopoverMenu3.0.0

更新内容：新增弹出窗插件

5.版本号：uexCamera-3.0.3

更新内容：* 优化插件改为arc，添加openInternal自定义相机接口
        * 新增openViewCamera自定义view模式相机接口


***
### 2016/03/12版本更新记录
####iOS引擎：
1. 版本号：ios_Engine_3.2_160219_01			

   更新内容：* 引擎新添share 调用系统分享接口

####iOS插件：
1. 版本号：uexScanner-3.1.6	

   更新内容：添加charset字段设置编码
   
2. 版本号：uexPopoverMenu3.0.0	

   更新内容：新弹出窗插件
***
### 2016/03/12版本更新记录
####iOS引擎：
1. 版本号：ios_Engine_3.3_160307_01

   更新内容：* uexWindow添加获取window宽高的方法

####iOS插件：
1. 版本号：uexLoadingView-3.0.5
   更新内容：解决空指针报错问题2. 版本号：uexKeyChain-3.0.2
   更新内容：添加接口getDeviceUniqueIdentifier3. 版本号：uexSlidePager-3.0.14
   更新内容：openSlidePager接口添加option参数4. 版本号：uexCamera-3.0.3
   更新内容：插件改为arc，添加openInternal自定义相机接口，添加openViewCamera自定义view模式相机接口5. 版本号：uexImage-3.0.9
   更新内容：修复pick接口选取拍摄的照片时方向可能不正确的bug6. 版本号：uexMobSMS-3.0.0
   更新内容：新增iOS短信验码证插件
***
### 2016/03/08版本更新记录
####iOS插件：
1.版本号：uexCreditCardRec-3.0.4
更新内容：* 新增支持iOS9

2.版本号：uexGestureUnlock-3.0.2
更新内容：* 修复maximumAllowTrialTimes拼写错误

3.版本号：uexPDFReader-3.0.5
更新内容：* 优化info.plist

4.版本号：uexActionSheet-3.0.7
更新内容：* 优化textNColor属性失效的bug

5.版本号：uexAreaPickerView-3.0.5	
更新内容：* 优化clean时的崩溃问题

6.版本号：uexButton-3.0.5	
更新内容：* 优化uexButton动态库在低版本手机上无法调用的问题

7.版本号：uexButton-3.0.5	
更新内容：* 优化uexButton动态库在低版本手机上无法调用的问题

8.版本号：uexChatKeyboard-3.0.21	
更新内容：* 优化自定义功能按钮和表情按钮重新打开会弹出键盘的bug

9.版本号：uexCoverFlow2-3.0.3
更新内容：* 新增新版Xcode重新编译,支持arm64

10.版本号：uexEditDialog-3.0.2
更新内容：* 新增新版Xcode重新编译,支持arm64

11.版本号：uexHexagonal-3.0.3
更新内容：* 新增新版Xcode重新编译,支持arm64

12.版本号：uexIndexBar-3.0.7
更新内容：* 新增索引表可以设置是否随网页滑动

13.版本号：uexSearchBarView-3.0.1
更新内容：* 新增搜索框

14.版本号：uexSlidePager-3.0.12
更新内容：* 优化适配iPhone6和iPhone6 Plus

15.版本号：uex3DTouch-3.0.1
更新内容：* 优化3DTouch 功能插件

16.版本号：uexCall-3.0.3
更新内容：* 优化uexCall.call方法取消"应用程序需要拨打电话,是否确定拨号?"的提示

17.版本号：uexCamera-3.0.2
更新内容：* 优化插件改为arc，添加openInternal自定义相机接口，添加openViewCamera自定义view模式相机

18.版本号：uexClipboard-3.0.3
更新内容：* 优化被复制的文本包含换行符会导致插件异常的bug

19.版本号：uexDataBaseMgr-3.0.4
更新内容：* 优化uexDataBaseMgr插件IDE包创建表格失败的问题

20.版本号：uexDocumentReader-3.0.4
更新内容：* 优化读取txt文件乱码,无法读取xls文件的bug

21.版本号：uexJsonXmlTrans-3.0.1
更新内容：* 优化JsonXmlTrans 插件

22.版本号：uexKeyChain-3.0.1
更新内容：* 优化iOS钥匙串插件

23.版本号：uexLocalNotification-3.0.6
更新内容：* 优化info.plist

24.版本号：uexLocation-3.0.23
更新内容：* 优化为ARC工程

25.版本号：uexLog-3.0.4
更新内容：* 优化崩溃问题

26.版本号：uexSMS-3.0.2
更新内容：* 新增使用新版Xcode重新编译,支持arm64

27.版本号：uexSensor-3.0.4
更新内容：* 优化sendDataToJS时的崩溃问题

28.版本号：uexTouchID-3.0.1
更新内容：* 优化TouchID功能插件

29.版本号：uexZip-3.0.4
更新内容：* 优化类名ZipArchive为UexZipArchive,解决与引擎的类名冲突

30.版本号：uexSocketMgr-3.0.6
更新内容：* 优化使用base64格式传输数据ios发送不成功的问题

31.版本号：uexUploaderMgr-3.0.14
更新内容：* 优化上传进度条达不到100%

32.版本号：uexXmlHttpMgr-3.0.15
更新内容：* 优化info.plist
***

### 2016/03/02版本更新记录
####iOS引擎：
 版本号：ios_Engine_3.2_160224_01 更新内容：* 优化config.xml中配置的起始页面不支持https://协议的问题
 
####iOS插件：
1. 版本号：uexCalendarView-3.0.5  更新内容：* 优化uexCalendarView切换年份时触发click事件的bug2. 版本号：uexDownloaderMgr-3.0.14  更新内容：* 优化在复用窗口中使用时回调丢失的bug3. 版本号：uexInAppPurchase-3.0.0   更新内容：* 新增iOS内购插件4. 版本号： uexScrollPicture-3.0.4   更新内容：    * 优化手滑动的时候下面轮播点不变的bug;    * 优化为不主动自动轮播    * 优化了轮播点颜色                                                                                       * 优化了viewId传Number会挂掉的bug    5. 版本号： uexAudio-3.0.14   更新内容：* 优化audio录的本地录音传到服务器上放不了bug6. 版本号： uexEasemob-3.0.19   更新内容：* 优化onMessageSent中群组消息的from和to参数不正确的问题7. 版本号： uexSecurityKeyboard-3.0.0   更新内容：* 新增uexSecurityKeyboard安全键盘输入框插件   
  ***

### 2016/02/24版本更新记录
####iOS插件：
1. 版本号：uexDevice-3.0.7
    更新内容：* openSetting接口支持打开推送通知设置2. 版本号：uexControl-3.0.15   更新内容：* 优化无法打开带配置的日期选择器的BUG3. 版本号：uexSegmentControl-3.0.3   更新内容：* 优化onItemClick接口回调参数与文档及安卓不一致的BUG
   ***
### 2016/02/22版本更新记录
####iOS插件：
1. 版本号：uexDevice-3.0.6   更新内容：* 新增判断功能是否开启,以及打开设置界面接口2. 版本号：uexScrollPicture-3.0.3   更新内容：* 优化回调可能会被错误触发的bug3. 版本号：uexImage-3.0.8   更新内容：* 优化openPicker接口打开相册时，默认滑动至最底端，以显示最新拍摄的照片4. 版本号：uexFileMgr-3.0.23   更新内容：* 优化工程为ARC;修复在复用窗口中使用时回调丢失的bug  ***

### 2016/01/26版本更新记录
####iOS引擎：
 版本号：ios_Engine_3.2_160121_01 更新内容：
 * 优化IDE下首次启动读取document下的widget包. * 优化iOS窗口打开路径问题,4.0云平台配置项引擎修改
####iOS插件：
1. 版本号：uexSina-3.0.6  更新内容：* 新增uexSina添加分享图片可以分享网络图片的功能2. 版本号：uexWheel-3.0.14  更新内容：* 优化和天翼RTC插件一起打包时会冲突的bug    3. 版本号：uexAudio-3.0.13  更新内容：  * uexAudio插件有更新，优化amr格式文件路径不存在时播放崩溃  * uexAudio优化播放AMR音频完成时没有回调的问题4. 版本号：uexInputTextFieldView-3.0.7  更新内容： * 优化索引bundle内资源的路径错误而无法显示图片背景的BUG
  ***

### 2016/01/11版本更新记录
####iOS引擎：
 版本号：ios_Engine_3.2_160109_01 更新内容：* 优化uexWindow.createProgressDialog uexWindow.destroyProgressDialog 这2个接口 现在支持iOS
####iOS插件：
1. 版本号：uexBluetoothLE-3.0.4
   更新内容：* 优化cbInit回调参数错误的bug
2. 版本号：uexContact-3.0.7
   更新内容：* 新增searchItem接口增加返回信息条数配置;addItem接口增加是否弹出提示框配置
3. 版本号：uexESurfingRtc-3.0.8
   更新内容：* 新增onGlobalStatus与cbCallStatus
4. 版本号：uexGaodeMap-3.0.9
   更新内容：
   * 新增IDE支持   * 优化接口设置APIKey   * 优化和高德导航冲突的问题
***

### 2016/01/07版本更新记录
####iOS插件：
1.版本号：uexWeiXin-3.0.19  更新内容：
   * 优化getWeiXinLoginAccessToken失效的bug
 * 优化getLoginAccessToken在多次调用时无法刷新code导致结果异常的bug ***

### 2015/12/31版本更新记录
####iOS插件：
1. 版本号：uexEasemob-3.0.17     更新内容：* 优化getMessageHistory接口传入startMsgId但pagesize为0时取不到所有messages的问题2. 版本号：uexWeiXin-3.0.18     更新内容：    * 重写回调相关代码，支持setCallbackWindowName接口    * 添加IDE支持 ***

### 2015/12/26版本更新记录
####iOS插件：
1. 版本号：uexImage-3.0.5     更新内容：    * 新增接口setIpadPopEnable    * 添加IDE支持2. 版本号：uexScanner-3.1.4     更新内容：    * 重构:改用ZXing识别二维码    * 添加IDE支持3. 版本号：uexChart-3.0.3     更新内容：    * barChart和lineChart新增option参数    * 使用Swift2.1编译，支持IDE ***

### 2015/12/19版本更新记录
####iOS插件：
1. 版本号：uexChatKeyboard-3.0.20   更新内容：    * 修复确定按钮出现AppCan背景图的问题    * 修改键盘弹出时页面弹动    * 修复自定义功能按钮和表情按钮重新打开会弹出键盘的bug2. 版本号：uexEasemob-3.0.16   更新内容：修复cbGetGroup回调结构和Android不一致的问题3. 版本号：uexGestureUnlock-3.0.1   更新内容：新增4. 版本号：uexUmeng-3.0.1   更新内容：新增 5. 版本号：uexUnionPay-3.0.0   更新内容：新增  ***

### 2015/12/07版本更新记录
####iOS插件：
1. 版本号：uexDownloaderMgr-3.0.12     更新内容：修改了下载时进度条不动的BUG   2. 版本号：uexUploaderMgr-3.0.13     更新内容：修改了上传进度条达不到100%3. 版本号：uexLocation-3.0.22     更新内容：更改为ARC工程
***

### 2015/12/04版本更新记录
####iOS插件：
1. 版本号：uexAudio-3.0.11
   更新内容：支持后台播放音频，需配置相关权限
***

### 2015/12/03版本更新记录
####iOS引擎：
 版本号：ios_Engine_3.2_151203_01 更新内容：修复应用通过点击APNs推送启动时，pushNotify不触发的问题
####iOS插件：
1. 版本号：uexJPush-3.0.7
   更新内容：现在应用在后台时，点击推送，会正确的触发onReceiveNotificationOpen；
***

### 2015/11/30版本更新记录
####iOS插件：
1. 版本号：uexSina-3.0.6
   更新内容：替换SinaSDK，重写授权登陆相关接口；新增login、logout、getUserInfo接口；2. 版本号：uexChatKeyboard-3.0.17
   更新内容：修改了点击发送不收回键盘
***
### 2015/11/23版本更新记录
####iOS插件：
1. 插件名称及版本号：uexDownloaderMgr-3.0.11       更新内容： 
	* 修改请求的变量	* 修改clean方法	* 验证的请求头的中的appid与key不匹配	* 判断当前的验证的请求头的属于的应用
	
2. 版本号：uexBaiduMap-3.1.15   更新内容：修改插件，使其支持config配置APIKey***
### 2015/11/19版本更新记录
####iOS插件：
1. 插件名称及版本号：uexImage-3.0.3       更新内容： 删去资源包中多余的info.plist
***
### 2015/11/13版本更新记录
####iOS引擎：
版本号：ios_Engine_3.2_151113_01
更新内容：* 现在在root页面加载完成后 经过500ms的延时 启动图才会关闭。解决在部分设备上，应用启动之后会黑屏闪一下的问题。
####iOS插件：
1. 插件名称及版本号：uexKeyChain-3.0.0    更新内容： 新增（仅ios）更新到文档和插件中心 
2. 插件名称及版本号：uexWeiXin-3.0.17
   更新内容： * 新增一版微信登陆、获取acess_token、获取用户信息acess_token、校验acess_token、刷新acess_token接口；
### 2015/10/30版本更新记录
####iOS引擎： 1. 插件名称及版本号：ios_Engine_3.1_151109_01       更新内容： 
        更新：	* 引擎自带的系统提示现在已经国际化了（目前支持简体中文和英文）	* (for 插件开发者) EUtility工具类添加了几个非常有用的接口，方便插件管理资源文件 插件国际化 以及插件进行js回调	* (for 插件开发者) 插件EUEx类现在可以通过类方法+(void)application:performActionForShortcutItem:completionHandler: 和+(void)application:didReceiveRemoteNotification:fetchCompletionHandler: 捕获到相应的系统事件	* (for 插件开发者) 插件EUEx类现在可以通过类方法+(void)rootPageDidFinishLoading 捕获到 root网页加载完成 这个AppCan事件	* 引擎现在支持3DTouch长按手势，可以实现快速跳转到APP指定页面的效果（详见插件uex3DTouch)
		优化:	* 优化了openMultiPopover接口，现在此接口会先打开当前指定页面，再预加载其他的页面，因此大大减少了从调用此接口到显示页面的时间。	* 现在打包得到的APP文件明显变小了	* 优化了APP的启动速度，启动时间及显示启动图的时间均变短了
		修复bugs:	* 修复Xcode7以及iOS9的诸多兼容性bug	* 修复在开启侧滑关闭后uexWindow.onWindowAppear和uexWindow.onWindowDisappear可能会失效的bug	* 修复听云检测到的一个可能会导致APP崩溃的bug####iOS插件： 1. 插件名称及版本号：uex3DTouch-3.0.0       更新内容： 新增 
    ***
### 2015/10/30版本更新记录
####iOS插件：
1. 插件名称及版本号：uexAreaPickerView-3.0.4       更新内容： 修复clean时崩溃的问题   2. 插件名称及版本号：uexQQ-3.0.12       更新内容：删去腾讯SDK中的info.plist,解决上架AppStore出现ERROR ITMS-90049的问题
    3. 插件名称及版本号：uexImage-3.0.1       更新内容：    * 删掉bundle中的info.plist 解决上架AppStore会提示Error:90535的问题    * 修复openCropper没有国际化的问题4. 插件名称及版本号：uexTestinCrash-3.0.1       更新内容： 升级SDK至2.0.6
    5. 插件名称及版本号：uexEasemob-3.0.15       更新内容：    * SDK版本更新至V2.2.0r1    * 修复iOS和Android之间互发消息时ext属性丢失的bug6. 插件名称及版本号：uexCalendarView-3.0.2       更新内容： 删除info.plist7. 插件名称及版本号：uexControl-3.0.13       更新内容： 删除info.plist8. 插件名称及版本号：uexEmail-3.0.5       更新内容： 删除info.plist9. 插件名称及版本号：uexFileMgr-3.0.18       更新内容： 删除info.plist10. 插件名称及版本号：uexBaiduMap-3.1.14       更新内容： 删除info.plist11. 插件名称及版本号：uexLocalNotification-3.0.5       更新内容： 删除info.plist12. 插件名称及版本号：uexLocation-3.0.21       更新内容： 删除info.plist13. 插件名称及版本号：uexPDFReader-3.0.4       更新内容： 删除info.plist14. 插件名称及版本号：uexXmlHttpMgr-3.0.14       更新内容： 删除info.plist   
15. 插件名称及版本号：uexJPush-3.0.6       更新内容：修复root页面回调失效的bug16. 插件名称及版本号：uexScrollPicture-3.0.1       更新内容：支持加载网络路径的图片
***

### 2015/10/27版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_151027_01      更新内容：修复close回到root页面可能会导致闪退的bug
  ***

### 2015/10/26版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_151026_01      更新内容：修改4.0数据统计的方法
  ***
### 2015/10/23版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_151022_01      更新内容：
   * 开发工具类EUtility添加国际化方法，支持插件国际化;   * 添加接口uexWindow.disturbLongPressGesture 


####iOS插件：
 1. 插件名称及版本号：uexBluetoothLE-3.0.2       更新内容：修复一个可能会导致Characteristic写入失败的bug 2. 插件名称及版本号：uexJPush-3.0.5        更新内容：    * 新增接口 disableLocalNotificationAlertView  禁止显示前台本地通知提示框 (仅iOS)    * onReceiveNotification 接口添加参数 isAPNs:,//Boolean (仅iOS)  推送是否来自APNs    * onReceiveNotification 现在也可以接收本地通知    * onReceiveNotificationOpen 接口添加参数 isAPNs:,//Boolean (仅iOS)  推送是否来自APNs    * onReceiveNotificationOpen 现在也会被 "点击本地通知打开APP” 这一事件触发  3. 插件名称及版本号：uexQQ-3.0.11       更新内容：    * 修复了一个在传参错误的情况下可能会导致闪退的bug    * sdk版本升级至2.9.2，修复了若干Xcode7+iOS9下的兼容性bug 4. 插件名称及版本号：uexTouchID-3.0.0       更新内容：新增   5. 插件名称及版本号：uexImage-3.0.0       更新内容：新增  6. 插件名称及版本号：uexBaiduMap-3.1.13       更新内容：国际化7. 插件名称及版本号：uexCalendarView-3.0.1       更新内容：国际化8. 插件名称及版本号：uexControl-3.0.12       更新内容：国际化9. 插件名称及版本号：uexEmail-3.0.4       更新内容：国际化10. 插件名称及版本号：uexFileMgr-3.0.17       更新内容：国际化11. 插件名称及版本号：uexLocalNotification-3.0.4       更新内容：国际化12. 插件名称及版本号：uexLocation-3.0.20       更新内容：国际化13. 插件名称及版本号：uexPDFReader-3.0.3       更新内容：国际化14. 插件名称及版本号：uexXmlHttpMgr-3.0.13       更新内容：国际化

### 2015/10/16版本更新记录
####iOS插件：
 1. 插件名称及版本号：uexBaiduMap-3.1.12
       更新内容：修复onMapLongClickListener回调结果异常的bug
 2. 插件名称及版本号：uexDevice-3.0.3        更新内容：设备列表更新
 3. 插件名称及版本号：uexEasemob-3.0.14
       更新内容：
    * cbLogin 返回信息修改为”msg” 与文档一致    * cbLogin 和cbRegisterUser 会返回失败时的错误信息了     4. 插件名称及版本号：uexEmail-3.0.3
       更新内容：修复设置多个附件时,不能正确读取协议路径文件的bug
 5. 插件名称及版本号：uexQQ-3.0.10
       更新内容：修复使用腾讯第三方TencentOpenApi_IOS_Bundle.bundle,用Xcode7上传archive的时候报unexpected CFBundleExecutable Key的错误.
***
### 2015/10/10版本更新记录
####iOS插件：
 1. 插件名称及版本号：uexChatKeyboard-3.0.12
       更新内容：修复关闭输入法后窗口显示不正常的bug
 2. 插件名称及版本号：uexDownloaderMgr-3.0.7
        更新内容：xcode7修正
 3. 插件名称及版本号：uexBluetoothLE-3.0.1
       更新内容：
    * 修改读写的字符串均为为Base64编码
    * 添加cbInit回调     4. 插件名称及版本号：uexFileMgr-3.0.16
       更新内容：getFileListByPath不再返回其子目录下的文件路径、不再包含多余的'/'
***

### 2015/9/25版本更新记录
####iOS插件：
1. 插件名称及版本号：uexGaodeMap-3.0.7       更新内容：
    * AddCircleOverlay中 修改默认lineDash值为NO
    * 当回调的json结构为String时，不再转义一次
    
2. 插件名称及版本号：uexUnisound-3.0.0       更新内容：新增

3. 插件名称及版本号：uexJsonXmlTrans-3.0.0       更新内容：新增
 
***
### 2015/9/21版本更新记录
####iOS插件：
1. 插件名称及版本号：uexGaodeMap-3.0.6       更新内容：open接口增加地图是否随网页滚动接口
***
### 2015/9/18版本更新记录
####iOS引擎：            版本号：ios_Engine_3.1_150918_01      更新内容：EUtility添加方法bundleForPlugin


####iOS插件：
 1. 插件名称及版本号：uexChatKeyboard-3.0.10       更新内容：
    * 新增 onKeyBoardShow监听方法 changeWebViewFrame方法(仅iOS) hideKeyboard方法 onCommitJson方法	* open接口新增参数inputMode默认输入方式。
 2. 插件名称及版本号：uexFileMgr-3.0.12       更新内容：新增方法search 搜索文件/文件夹

 3. 插件名称及版本号：uexBaiduNavi-3.0.0       更新内容：新增
***

### 2015/9/11版本更新记录
####iOS插件：
 1. 插件名称及版本号：uexXmlHttpMgr-3.0.12
       更新内容：setAppVerify新增加appId的信息
 2. 插件名称及版本号：uexUploaderMgr-3.0.12
        更新内容：修改clean方法,setAppVerify新增加appId的信息
 3. 插件名称及版本号：uexQQ-3.0.9
       更新内容：修复取消登录时cbLogin不触发的bug     4. 插件名称及版本号：uexLog-3.0.3
       更新内容：修复崩溃问题
 5. 插件名称及版本号：uexJPush-3.0.4
       更新内容：新增接口setBadgeNumber
 6. 插件名称及版本号：uexDownloaderMgr-3.0.6
       更新内容：setAppVerify新增加appId的信息
***    
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
