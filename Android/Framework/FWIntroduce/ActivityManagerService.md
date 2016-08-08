
#ActivityManagerService

Android核心服务，负责系统四大组件的启动、切换、调度等，还负责应用进程的管理和调度。

##AMS中几个关键概念

- **ProcessRecord:** 应用进程
- **ActvitiyThread:**  代表进程的主线程，将应用进程和AMS建立双向连接
- **ActivityRecord:** 代表一个Activity
- **ActivityStack:**  Activity栈，栈顶的Activity是处于resume状态
- **Task:** 任务一个Task由1个或多个Activity组成
