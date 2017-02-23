---
layout: post
title: Visual Studio Code 快捷键汇总之Windows平台
category: 编辑器
tags: [编辑器,IDE,快捷键]
---

Visual Studio Code(vs code)快捷键汇总之Windows平台

作者：iwenli

GitHub：[https://github.com/iwenli](https://github.com/iwenli)

# 1.序言

本篇文字是从vs code(Visual Studio Code的简称)官方文档翻译摘录出来的，欢迎大家指正。
官方链接：http://code.visualstudio.com/docs/customization/keybindings#_editorwindow-management

下面提供一个可打印版本的pdf下载：

+ [Windows](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf)
+ [macOS](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf)
+ [Linux](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf)

# 2.Windows版参考快捷键总结

> 注意:下面所有的快捷键都是按标准的美国键盘布局罗列的， 如果你使用不同的键盘布局，[请阅读这里](http://code.visualstudio.com/docs/customization/keybindings#_keyboard-layouts)

## 2.1.基本编辑

|快捷键|命令|命令id|
|:-|:-:|:-:|
|Ctrl + X|剪切(空选择)|`editor.action.clipboardCutAction`|
|Ctrl + C|复制选择(空行)|`editor.action.clipboardCopyAction`|
|Ctrl + Shift + K|删除一行|`editor.action.deleteLines`|
|Ctrl + Enter|当前行下面插入一行|`editor.action.insertLineAfter`|
|Ctrl + Shift + Enter|当前行上面插入一行|`editor.action.insertLineBefore`|
|Alt + Down|当前行和下一行交换位置|`editor.action.moveLinesDownAction`|
|Alt + Up|当前行和上一行交换位置|`editor.action.moveLinesUpAction`|
|Shift + Alt + Down|复制当前行到上一行|`editor.action.copyLinesDownAction`|
|Shift + Alt + Up|复制当前行到下一行|`editor.action.copyLinesUpAction`|
|Ctrl + D|匹配下一个当前选择的内容|`editor.action.addSelectionToNextFindMatch`|
|Ctrl + K Ctrl + D|移动到匹配的下一个当前选择的内容|`editor.action.moveSelectionToNextFindMatch`|
|Ctrl + U|撤消最后光标操作|`cursorUndo`|
|Shift + Alt + I|将光标移动到选择内容的结尾|`editor.action.insertCursorAtEndOfEachLineSelected`|
|Ctrl + Shift + L|选择当前匹配到的所有选择|`editor.action.selectHighlights`|
|Ctrl + F2|选择当前匹配到的所有选择(感觉跟上一个没有什么区别)|`editor.action.changeAll`|
|Ctrl + I|选择当前行|`expandLineSelection`|
|Ctrl + Alt + Down|插入光标下面|`editor.action.insertCursorBelow`|
|Ctrl + Alt + Up|上面插入光标|`editor.action.insertCursorAbove`|
|Ctrl + Shift + \ |跳转到匹配的括号|`editor.action.jumpToBracket`|
|Ctrl + ]|增加缩进|`editor.action.indentLines`|
|Ctrl + [|减少缩进|`editor.action.outdentLines`|
|Home|移动光标到行首|`cursorHome`|
|End|移动光标到行末|`cursorEnd`|
|Ctrl + End|定位到页面底部|`cursorBottom`|
|Ctrl + Home|定位到页面顶部|`cursorTop`|
|Ctrl + Down|整个页面下滚一行|`scrollLineDown`|
|Ctrl + Up|整个页面上滚一行|`scrollLineUp`|
|Alt + PageDown|切换下一个页面|`scrollPageDown`|
|Alt + PageUp|切换上一个页面|`scrollPageUp`|
|Ctrl + Shift + [|折叠代码块|`editor.fold`|
|Ctrl + Shift + ]|展开代码块|`editor.unfold`|
|Ctrl + K Ctrl + [|折叠子区域代码块|`editor.foldRecursively`|
|Ctrl + K Ctrl + ]|展开子区域代码块|`editor.unfoldRecursively`|
|Ctrl + K Ctrl + 0|折叠所有代码块|`editor.foldAll`|
|Ctrl + K Ctrl + J|展开所有代码块|`editor.unfoldAll`|
|Ctrl + K Ctrl + C|添加多行注释|`editor.action.addCommentLine`|
|Ctrl + K Ctrl + U|删除多行注释|`editor.action.removeCommentLine`|
|Ctrl + /|添加单行注释|`editor.action.commentLine`|
|Shift + Alt + A|切换块注释|`editor.action.blockComment`|
|Ctrl + F|查找|`actions.find`|
|Ctrl + H|替换|`editor.action.startFindReplaceAction`|
|F3|查找下一个|`editor.action.nextMatchFindAction`|
|Shift + F3|查找上一个|`editor.action.previousMatchFindAction`|
|Alt + Enter|选择出现的所有找到匹配|`editor.action.selectAllMatches`|
|Alt + C|切换找到区分大小写|`toggleFindCaseSensitive`|
|Alt + R|切换发现正则表达式|`toggleFindRegex`|
|Alt + W|切换找到整词|`toggleFindWholeWord`|
|Ctrl + M|使用Tab键切换设置焦点|`editor.action.toggleTabFocusMode`|
|unassigned|切换显示空白|`toggleRenderWhitespace`|
|Alt + Z|切换自动换行|`editor.action.toggleWordWrap`|


## 2.2.丰富的语言编辑

|快捷键|命令|命令id|
|:-|:-:|:-:|
|Ctrl + Space|触发显示|`editor.action.triggerSuggest`|
|Ctrl + Shift + Space|触发参数提示|`editor.action.triggerParameterHints`|
|Shift + Alt + F|格式的文档|`editor.action.formatDocument`|
|Ctrl + K Ctrl + F|格式选择|`editor.action.formatSelection`|
|F12|去定义|`editor.action.goToDeclaration`|
|Alt + F12|Peek的定义|`editor.action.previewDeclaration`|
|Ctrl + K F12|开放的定义|`editor.action.openDeclarationToTheSide`|
|Ctrl + .|快速修复|`editor.action.quickFix`|
|Shift + F12|显示引用|`editor.action.referenceSearch.trigger`|
|F2|重命名符号|`editor.action.rename`|
|Ctrl + Shift + .|替换为下一个值|`editor.action.inPlaceReplace.down`|
|Ctrl + Shift + ,|与先前的值替换|`editor.action.inPlaceReplace.up`|
|Shift + Alt + Right|展开AST选择|`editor.action.smartSelect.grow`|
|Shift + Alt + Left|缩小AST选择|`editor.action.smartSelect.shrink`|
|Ctrl + K Ctrl + X|修剪后的空白|`editor.action.trimTrailingWhitespace`|
|Ctrl + K M|改变语言模式|`workbench.action.editor.changeLanguageMode`|

## 2.3.导航

|快捷键|命令|命令id|
|:-|:-:|:-:|
|Ctrl + T|显示所有符号|`workbench.action.showAllSymbols`|
|Ctrl + G|跳转到行|`workbench.action.gotoLine`|
|Ctrl + P|快速打开文件|`workbench.action.quickOpen`|
|Ctrl + Shift+O|去象征……|`workbench.action.gotoSymbol`|
|Ctrl + Shift+M|显示的问题|`workbench.actions.view.problems`|
|F8|去下一个错误或警告|`editor.action.marker.next`|
|Shift + F8|去之前的错误或警告|`editor.action.marker.prev`|
|Ctrl + Shift + P|显示所有命令|`workbench.action.showCommands`|
|Ctrl + Shift + Tab|导航编辑历史|`workbench.action.openPreviousRecentlyUsedEditorInGroup`|
|Alt + Left|返回|`workbench.action.navigateBack`|
|Alt + Right|前进|`workbench.action.navigateForward`|

## 2.4.编辑/窗口管理

|快捷键|命令|命令id|
|:-|:-:|:-:|
|Ctrl + Shift + N|新窗口|`workbench.action.newWindow`|
|Ctrl + Shift + W|关闭窗口|`workbench.action.closeWindow`|
|Ctrl + F4|关闭编辑器|`workbench.action.closeActiveEditor`|
|Ctrl + K F|关闭文件夹|`workbench.action.closeFolder`|
|未赋值|编辑器组之间循环|`workbench.action.navigateEditorGroups`|
|Ctrl + \|把编辑器|`workbench.action.splitEditor`|
|Ctrl + 1|焦点到离开编辑器组|`workbench.action.focusFirstEditorGroup`|
|Ctrl + 2|集中到一边编辑器组|`workbench.action.focusSecondEditorGroup`|
|Ctrl + 3|集中到正确的编辑器组|`workbench.action.focusThirdEditorGroup`|
|Ctrl + K Ctrl + Left|焦点到编辑器组在左边|`workbench.action.focusPreviousGroup`|
|Ctrl + K Ctrl + Right|焦点到编辑器组在右边|`workbench.action.focusNextGroup`|
|Ctrl + Shift + PageUp|移动编辑了|`workbench.action.moveEditorLeftInGroup`|
|Ctrl + Shift + PageDown|编辑器右移动|`workbench.action.moveEditorRightInGroup`|
|Ctrl + K Left|移动活跃编辑群离开了|`workbench.action.moveActiveEditorGroupLeft`|
|Ctrl + K Right|活动编辑器组右移动|`workbench.action.moveActiveEditorGroupRight`|


## 2.5.文件管理

|快捷键|命令|命令id|
|:-|:-:|:-:|
|Ctrl + N|新文件|`workbench.action.files.newUntitledFile`|
|Ctrl + O|打开文件…|`workbench.action.files.openFile`|
|Ctrl + S|保存|`workbench.action.files.save`|
|Ctrl + K S|保存所有|`workbench.action.files.saveAll`|
|Ctrl + Shift + S|另存为…|`workbench.action.files.saveAs`|
|Ctrl + F4|关闭|`workbench.action.closeActiveEditor`|
|未赋值|接近别人|`workbench.action.closeOtherEditors`|
|Ctrl + K W|关闭组|`workbench.action.closeEditorsInGroup`|
|未赋值|关闭其他组|`workbench.action.closeEditorsInOtherGroups`|
|未赋值|关闭组到左|`workbench.action.closeEditorsToTheLeft`|
|未赋值|关闭组到右|`workbench.action.closeEditorsToTheRight`|
|Ctrl + K Ctrl + W|关闭所有|`workbench.action.closeAllEditors`|
|Ctrl + Shift + T|重新打开关闭编辑器|`workbench.action.reopenClosedEditor`|
|Ctrl + K Enter|保持开放|`workbench.action.keepEditor`|
|Ctrl + Tab|打开下一个|`workbench.action.openNextRecentlyUsedEditorInGroup`|
|Ctrl + Shift + Tab|打开之前|`workbench.action.openPreviousRecentlyUsedEditorInGroup`|
|Ctrl + K P|复制活动文件的路径|`workbench.action.files.copyPathOfActiveFile`|
|Ctrl + K R|显示活跃的文件窗口|`workbench.action.files.revealActiveFileInWindows`|
|Ctrl + K O|在新窗口显示打开文件|`workbench.action.files.showOpenedFileInNewWindow`|
|未赋值|比较了文件|`workbench.files.action.compareFileWith`|


## 2.6.显示

|快捷键|命令|命令id|
|:-|:-:|:-:|
|F11|切换全屏|`workbench.action.toggleFullScreen`|
|Ctrl + K Z|禅模式开关|`workbench.action.toggleZenMode`|
|Escape Escape|离开禅模式|`workbench.action.exitZenMode`|
|Ctrl + =|放大|`workbench.action.zoomIn`|
|Ctrl + -|缩小|`workbench.action.zoomOut`|
|Ctrl + Numpad0|重置放大|`workbench.action.zoomReset`|
|Ctrl + B|切换栏可见性|`workbench.action.toggleSidebarVisibility`|
|Ctrl + Shift + E|显示浏览器/切换焦点|`workbench.view.explorer`|
|Ctrl + Shift + D|显示调试|`workbench.view.debug`|
|Ctrl + Shift + G|向Git|`workbench.view.git`|
|Ctrl + Shift + X|显示扩展名|`workbench.view.extensions`|
|Ctrl + Shift + U|显示输出|`workbench.action.output.toggleOutput`|
|Ctrl + Q|快速打开视图|`workbench.action.quickOpenView`|
|Ctrl + Shift + F|显示搜索|`workbench.view.search`|
|Ctrl + Shift + H|在文件中替换|`workbench.action.replaceInFiles`|
|Ctrl + Shift + J|切换搜索细节|`workbench.action.search.toggleQueryDetails`|
|Ctrl + Shift + C|打开新的命令提示符|`workbench.action.terminal.openNativeConsole`|
|Ctrl + Shift + V|切换减价预览|`markdown.showPreview`|
|Ctrl + K V|打开预览|`markdown.showPreviewToSide`|
|Ctrl + \`|集成终端切换|`workbench.action.terminal.toggleTerminal`|


## 2.7.首选项

|快捷键|命令|命令id|
|:-|:-:|:-:|
|未赋值|开放的用户设置|`workbench.action.openGlobalSettings`|
|未赋值|开放式工作区设置|`workbench.action.openWorkspaceSettings`|
|Ctrl + K Ctrl + S|打开键盘快捷键|`workbench.action.openGlobalKeybindings`|
|未赋值|打开用户代码片段|`workbench.action.openSnippets`|
|Ctrl + K Ctrl + T|选择颜色主题|`workbench.action.selectTheme`|
|未赋值|配置显示语言|`workbench.action.configureLocale`|


## 2.8.调试

|快捷键|命令|命令id|
|:-|:-:|:-:|
|F9|Toggle Breakpoint|`editor.debug.action.toggleBreakpoint`|
|F5|开始,继续|`workbench.action.debug.continue`|
|Ctrl + F5|开始(没有调试)|`workbench.action.debug.run`|
|F6|暂停|`workbench.action.debug.pause`|
|F11|进入|`workbench.action.debug.stepInto`|
|Shift + F11|走出|`workbench.action.debug.stepOut`|
|F10|跨过|`workbench.action.debug.stepOver`|
|Shift + F5|停止|`workbench.action.debug.stop`|
|Ctrl + K Ctrl + I|显示徘徊|`editor.action.showHover`|


## 2.9.任务

|快捷键|命令|命令id|
|:-|:-:|:-:|
|Ctrl + Shift + B|运行构建任务|`workbench.action.tasks.build`|
|未赋值|运行测试任务|`workbench.action.tasks.test`|


## 2.10.扩展

|快捷键|命令|命令id|
|:-|:-:|:-:|
|未赋值|安装扩展|`workbench.extensions.action.installExtension`|
|未赋值|显示安装的扩展|`workbench.extensions.action.showInstalledExtensions`|
|未赋值|展示过时的扩展|`workbench.extensions.action.listOutdatedExtensions`|
|未赋值|显示推荐的扩展|`workbench.extensions.action.showRecommendedExtensions`|
|未赋值|受欢迎的扩展|`workbench.extensions.action.showPopularExtensions`|
|未赋值|更新所有的扩展|`workbench.extensions.action.updateAllExtensions`|


# 3.尾页

>之前一直都是用visualstudio做开发的，最近用了vsc感觉很棒，所以来研究一下，如果有错误的地方，大家下发评论指正，我也会第一时间更正哈。