## No such file or directory

github下载的开源项目打开后提示：diff: /../Podfile.lock: No such file or directory...

如下：

```bash
diff: /../Podfile.lock: No such file or directory
diff: /Manifest.lock: No such file or directory
error: The sandbox is not in sync with the Podfile.lock. Run 'pod install' or update your CocoaPods installation.
```

如图所示：

![01](https://github.com/Ranch2014/iOS-Problems/blob/master/pics/01.png)



- 原因

项目使用了开源框架，下载项目时被忽略了。



- 解决方法

终端进入到项目的目录，然后 `pod install` 下载相关开源框架即可。