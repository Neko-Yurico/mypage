# Android Studio SD卡访问权限

~~0、将android版本升级至6.0以上~~

1、在 `AndroidManifext.xml` 的 `manifest` 块内添加如下代码

```
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.MOUNT_UNMOUNT_FILESYSTEMS"/>
```

其分别表示 SD 卡的写，读和创建/删除文件权限

2、在 `MainActivity` 中将 `setRegist();` 方法注释掉或者删除

3、运行

4、在AVD中进入 `Settings—Apps—你的应用—Permissions` 并将 `	storage` 勾选上

5、再次运行

