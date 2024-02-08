# Douyin-Unfollow-Tools-Android
Android微信识别谁关闭了朋友圈-自动化脚本

# 特点
- 代码精简，纯本地操作，隐私无忧，只是纯手动操作的替代，无安全风险。
- 脚本只是通过微信Android App的布局识别，无需登录微信账号，无需微信授权。
- 通过官方Android Debug Bridge（adb）获取布局精准识别页面中的按钮位置进行操作。
- 目前只兼容简体中文。

# 环境要求
- 操作系统支持：Windows/Mac/Linux
- 手机要求：Android
- 测试通过的微信Android版本：8.0.42，其他版本未测试
- 需要安装 [adb](https://developer.android.google.cn/tools/releases/platform-tools?hl=zh-cn) 并放置到环境目录下
- 需要安装 Python3 并放置 python3 到环境目录下（Mac已自带，Windows需[手动安装](https://www.python.org/downloads/windows/)）

# 支持页面
1. 通讯录tab页

# 注意事项
1. 划到最底部会自动停止并输出结果。
2. 会从当前页面能看到的第一个好友开始，如果在最顶部，就是从字母A目录头后开始。
3. 每滑动下一页前会自动总结到目前的结果，不会导致中断完全看不到已跑过的结果。
4. 随时可以Ctrl+C停止脚本。

# 运行方式
1. 打开手机微信Android App
2. 切到通讯录tab页
3. 电脑通过USB连接Android手机
4. 在Android手机上启用「开发者模式」：一般位于 设置 > 关于手机 > 软件信息 > 版本号，连续点按版本号七次，会提示已成功开启开发者选项
5. 在Android手机上打开「高级设置」-「开发者选项」-「USB调试开关」
6. 在手机弹出的弹窗中确认开启调试开关并信任当前主机
7. 在Mac上打开“终端”；或在Windows打开“命令提示符”：Windows键+R > 输入"cmd" > 回车
8. 进入本工程的根目录：在“终端”或“命令提示符”窗口中输入“cd + 空格”，然后把工程目录用鼠标拖进窗口中，再点击回车即可
9. 在“终端”或“命令提示符”窗口中输入`python3 detect.py`，回车

# 打赏
<img src="./WeChat_QR_Code.jpg" alt="WeChat_QR_Code" height="400px" />
