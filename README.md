# 阻止下载安装 Windows 10 功能更新

· 按 Windows + R 打开 “运行”，然后键入 “ Regedit”，然后单击 “确定”（如果出现 UAC 提示，请单击 “是”）

· 导航到 “ HKEY_LOCAL_MACHINE \ SOFTWARE \ Policies \ Microsoft \ Windows \ WindowsUpdate”

· 右键单击 “ WindowsUpdate”，然后导航到 “新建”>“ DWORD（32 位）”值

· 将 DWORD 命名为 “ TargetReleaseVersion”（不带引号），并将其值设置为 “ 1”（不带引号）

· 右键单击 “ WindowsUpdate”，然后导航到 “新建”>“字符串值”

· 将字符串值命名为 “ TargetReleaseVersionInfo”（不带引号），并将其值设置为用户要使用的 Windows 10 版本。例如，如果用户不想更新到 Windows 10 v2004 并希望坚持使用 1909，则将 “ 1909”（不带引号）作为值
