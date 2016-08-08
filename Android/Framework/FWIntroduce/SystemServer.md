
#SystemServer

SystemServer是虚拟机启动后运行的第一个java进程

SystemServer启动其他系统服务,这些系统服务都是以一个线程的方式存在于SystemServer进程中

##SystemServer中启动服务列表

- **EntropyService:** 提供伪随机数
- PowerManagerService 电源管理服务
- ActivityManagerService  最核心的服务之一,管理Activity
- TelephonyRegistry 通过该服务注册电话模块的事件响应,比如重启、关闭、启动等
- PackageManagerService 程序包管理服务
- AccountManagerService 账户管理服务，是指联系人账户,而不是Linux系统的账户
- ContentService  ContentProvider服务，提供跨进程数据交换
- BatteryService  电池管理服务
- LightsService 自然光强度感应传感器服务
- VibratorService 震动器服务
- AlarmManagerService 定时器管理服务,提供定时提醒服务
- WindowManagerService  Framework最核心的服务之一,负责窗口管理
- BluetoothService  蓝牙服务
- DevicePolicyManagerService  提供一些系统级别的设置及属性
- StatusBarManagerService 状态栏管理服务
- ClipboardService  系统剪切板服务
- InputMethodManagerService 输入法管理服务
- NetStatService  网络状态服务
-NetworkManagementService 网络管理服务
-ConnectivityService  网络连接管理服务
- AccessibilityManagerService 辅助管理程序截获所有的用户输入,并根据这些输入给用户一些额外的反馈，起到辅助的效果
- MountService  挂载服务，可通过该服务调用Linux层面的mount程序
- NotificationManagerService  通知栏管理服务,Android中的通知栏和状态栏在一起，只是界面上前者在左边，后者在右边
- DeviceStorageMonitorService 磁盘空间状态检测服务
- LocationManagerService  地理位置服务
- SearchManagerService  搜索管理服务
- DropBoxManagerService 通过该服务访问Linux层面的Dropbox程序
- WallpaperManagerService 墙纸管理服务，墙纸不等同于桌面背景，在View系统内部，墙纸可以作为任何窗口的背景
- AudioService  音频管理服务
- BackupManagerService  系统备份服务
- AppWidgetService  Widget服务
- RecognitionManagerService 身份识别服务
- DiskStatsService  磁盘统计服务
