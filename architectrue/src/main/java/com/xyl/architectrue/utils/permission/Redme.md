权限请求策略
下面提供一种我认为还不错的策略
在需要某权限的Activity的 onStart() 中去请求权限
在 onRequestPermissionsResult 回调中,如果用户点击了拒绝,则继续请求权限
如果用户点击了不再提醒,则弹出自定义对话框,引导用户手动去开启权限,如果用户不授权,则退出当前页面
注意:适用于没有权限就无法使用该功能的情况

(笔记中有代码)
