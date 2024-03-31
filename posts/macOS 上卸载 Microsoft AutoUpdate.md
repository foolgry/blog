2024-03-28

#mac

Microsoft AutoUpdate是微软为了自动更新自己的软件搞出来的一个软件，如果你装过 edge 浏览器，就会发现也同时安装了这个，卸载 edge 并不会同时卸载这个软件。

要在macOS上卸载Microsoft AutoUpdate，可以采取几种不同的方法。以下是一些有效的方法：

### 方法一：设置权限不可访问

1. 打开终端。
2. 输入以下命令，然后按回车键：

   ```bash
   cd /Library/Application\ Support/Microsoft/MAU2.0
   sudo chmod 000 Microsoft\ AutoUpdate.app
   ```

3. 输入您的密码。这样，Microsoft AutoUpdate.app就没有执行权限了[1]。

### 方法二：删除Microsoft AutoUpdate

1. 打开访达。
2. 使用快捷键：`command（⌘）+⇧+G`，或者顶部菜单，选择“前往”——“前往文件夹”。
3. 在弹出的对话框中输入以下路径，然后点击“前往”：

   ```
   /Library/Application Support/Microsoft/
   ```

4. 删除文件夹`MAU2.0`，或者直接删除`Microsoft AutoUpdate.app`[1][2]。

### 方法三：通过系统偏好设置禁用通知

1. 点击屏幕顶部的苹果菜单，选择“系统偏好设置” > “通知”。
2. 找到Microsoft Update Assistant并关闭它[3]。

### 方法四：使用MacKeeper管理应用更新

如果您想要更有效地管理应用更新，可以考虑使用MacKeeper的Update Tracker功能。这个功能可以在您点击时通知您更新，并允许您一次性更新多个应用[3]。

### 方法五：使用AppCleaner卸载

1. 安装并打开AppCleaner。
2. 打开访达，按`Cmd+Shift+G`，粘贴路径`/Library/Application Support/Microsoft/MAU2.0/`。
3. 将`Microsoft AutoUpdate.app`拖到AppCleaner中进行删除[6]。

选择适合您需求的方法进行操作。如果您不再使用Microsoft的应用，或者希望手动管理这些应用的更新，卸载Microsoft AutoUpdate可以是一个好选择。

Citations:
[1] https://juejin.cn/post/6911190158469496840
[2] https://blog.csdn.net/weixin_50657813/article/details/124475225
[3] https://mackeeper.com/blog/stop-microsoft-autoupdate-on-mac/
[4] https://juejin.cn/post/7091942430777278478
[5] https://osxdaily.com/2019/07/20/how-delete-microsoft-autoupdate-mac/
[6] https://apple.stackexchange.com/questions/428234/how-to-remove-microsoft-autoupdate-from-macos
[7] https://www.macappbox.com/a/1177.html
[8] https://developer.baidu.com/article/details/2686266

