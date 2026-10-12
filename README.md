# JustSay installers

Download JustSay from **https://justsay.la**. This repository only hosts the
installer files so downloads are fast; it contains no source code.

| Platform | File |
| --- | --- |
| macOS (Apple silicon) | `JustSay-macOS.dmg` |
| Windows (64-bit) | `JustSay-Windows.exe` |
| Android | `JustSay-Android.apk` |

The files are in the [`latest` release](https://github.com/just-say/justsay-releases/releases/tag/latest).
`SHA256SUMS` lists their checksums:

```sh
shasum -a 256 -c SHA256SUMS --ignore-missing
```

## Installing

The installers are not yet signed by Apple or Microsoft, so the system asks you
to confirm once:

- **macOS**: open the `.dmg` and drag JustSay to Applications. Because the app is
  not notarized yet, macOS may say it is "damaged" and offer only the Trash. It is
  not damaged. Run this once in Terminal, then open the app normally:

  ```sh
  xattr -dr com.apple.quarantine /Applications/JustSay.app
  ```
- **Windows**: if SmartScreen appears, choose **More info**, then **Run anyway**.
- **Android**: allow installing from this source when asked, then open the APK.

Questions: contact@justsay.la

---

# JustSay 安装包

请从 **https://justsay.la** 下载 JustSay。这个仓库只存放安装包文件（让下载更快），
不包含任何源码。

- **macOS**：打开 `.dmg`，把 JustSay 拖进"应用程序"。因为暂未经过苹果公证，macOS 可能提示
  "已损坏"并只给"移到废纸篓"，其实文件完好。在"终端"里运行一次下面这条命令，然后正常打开即可：

  ```sh
  xattr -dr com.apple.quarantine /Applications/JustSay.app
  ```
- **Windows**：如果出现 SmartScreen，点"更多信息"，再点"仍要运行"。
- **Android**：按提示允许安装来自此来源的应用，再打开 APK。

安装包暂未做苹果和微软的签名，所以系统会要求你确认一次。
