# debug
windbg 

拦截窗口： 
bp CreateWindow 创建窗口 
bp CreateWindowEx(A) 创建窗口 
bp ShowWindow 显示窗口 
bp UpdateWindow 更新窗口 
bp GetWindowText(A) 获取窗口文本 

拦截消息框： 
bp MessageBox(A) 创建消息框 
bp MessageBoxExA 创建消息框 
bp MessageBoxIndirect(A) 创建定制消息框 
bp IsDialogMessageW 

拦截警告声： 
bp MessageBeep 发出系统警告声(如果没有声卡就直接驱动系统喇叭发声) 

拦截对话框： 
bp DialogBox 创建模态对话框 
bp DialogBoxParam(A) 创建模态对话框 
bp DialogBoxIndirect 创建模态对话框 
bp DialogBoxIndirectParam(A) 创建模态对话框 
bp CreateDialog 创建非模态对话框 
bp CreateDialogParam(A) 创建非模态对话框 
bp CreateDialogIndirect 创建非模态对话框 
bp CreateDialogIndirectParam(A) 创建非模态对话框 
bp GetDlgItemText(A) 获取对话框文本 
bp GetDlgItemInt 获取对话框整数值 

拦截剪贴板： 
bp GetClipboardData 获取剪贴板数据 

拦截注册表： 
bp RegOpenKey(A) 打开子健 
bp RegOpenKeyEx 打开子健 
bp RegQueryValue(A) 查找子健 
bp RegQueryValueEx 查找子健 
bp RegSetValue(A) 设置子健 
bp RegSetValueEx(A) 设置子健 

功能限制拦截断点： 
bp EnableMenuItem 禁止或允许菜单项 
bp EnableWindow 禁止或允许窗口 

拦截时间： 
bp GetLocalTime 获取本地时间 
bp GetSystemTime 获取系统时间 
bp GetFileTime 获取文件时间 
bp GetTickCount 获得自系统成功启动以来所经历的毫秒数 
bp GetCurrentTime 获取当前时间（16位） 
bp SetTimer 创建定时器 
bp TimerProc 定时器超时回调函数 
GetDlgItemInt 得指定输入框整数值 
GetDlgItemText 得指定输入框输入字符串 
GetDlgItemTextA 得指定输入框输入字符串 

拦截文件： 
bp CreateFileA 创建或打开文件 (32位) 
bp OpenFile 打开文件 (32位) 
bp ReadFile 读文件 (32位) 
bp WriteFile 写文件 (32位) 
GetModuleFileNameA 
GetFileSize 
Setfilepointer 
fileopen 
FindFirstFileA 
ReadFile 

拦截驱动器： 
bp GetDriveTypeA 获取磁盘驱动器类型 
bp GetLogicalDrives 获取逻辑驱动器符号 
bp GetLogicalDriveStringsA 获取当前所有逻辑驱动器的根驱动器路径
