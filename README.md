### 2021.01.28更新

- 原有的EFI不支持HDMI接口的输出，更新后EFI已支持

    <a href="./HDMI.md">点此查看HDMI教程</a>

- 解决HDMI接口休眠后唤醒有声音无画面问题

    添加启动参数`igfxonln=1`

- 关闭OpenCore debug模式（具体表现在每次启动都会生成log日志）

    ![](https://image.leejay.top/Fg3GZiGyTDvSZV1sx3qOdfFsE4rp)

### 配置
![](https://image.leejay.top/FhdyQFJ24FcxS65y1qDAScCB51Kp)

| 硬件        | 型号                          |
| ----------- | ----------------------------- |
| <b>CPU</b>  | <b>`i5-8400`</b>              |
| <b>主板</b> | <b>`MSI B360M`</b>            |
| <b>显卡</b> | <b>`HD630`</b>                |
| <b>内存</b> | <b>`威刚DDR4 2666`</b>        |
| <b>硬盘</b> | <b>`金士顿480G`</b>           |
| <b>网卡</b> | <b>`以太网卡（主板自带）`</b> |
| <b>网卡</b> | <b>`无`</b>                   |

---

### 适配系统(已测试)

- Macos 11.1 Big Sur
- Macos 10.15.7 Catalina

---

### TODO

- ~~DP/HDMI/DVI输出~~
- ~~CPU型号与核显型号（显存正常）正确识别~~
- ~~USB(3.0/2.0)识别正常~~
- ~~声卡驱动正常（HDMI下也正常）~~
- ~~睡眠与唤醒功能正常（HDMI也没问题）~~
- ~~imessage功能与三码正常~~
- OpenCore引导式有概率出现`StartImage failed - Aborted`问题
- 使用4k显示器，去除HIDPI功能（会导致掉帧的情况）
- 使用免驱独显，核显加速功能
- BCMP9436CD免驱网卡
- 更换SATA为m.2固态（暂定铠侠RC10 500GB）

### 相关资源链接

- [镜像：【黑果小兵】macOS BigSur 11.1 20C69 正式版 with Clover 5127原版镜像[双EFI版][UEFI and MBR]](https://blog.daliansky.net/macOS-BigSur-11.1-20C69-Release-version-with-Clover-5127-original-image-Double-EFI-Version-UEFI-and-MBR.html)

- [镜像：【黑果小兵】macOS Catalina 10.15.7 19H15 正式版 with Clover 5127原版镜像[双EFI版][UEFI and MBR]](https://blog.daliansky.net/macOS-Catalina-10.15.7-19H2-Release-version-with-Clover-5122-original-image-Double-EFI-Version-UEFI-and-MBR.html)

- [刻录工具：balenaEtcher](https://www.balena.io/etcher/)

- [OpenCore_0.6.5](https://github.com/acidanthera/OpenCorePkg/releases)

- [OpenCore 编辑器](https://github.com/ic005k/QtOpenCoreConfig/releases)

- [OpenCore document](https://dortania.github.io/OpenCore-Install-Guide/ktext.html)

- [OpenCore config在线校验](https://opencore.slowgeek.com/)

- [ProperTree中文版(基于python3)](https://gitee.com/btwise/ProperTree-CN)

- [低于4k屏幕开启hidpi(核显开启后可能存在掉帧情况)](https://github.com/xzhih/one-key-hidpi)

- [34寸带鱼屏开启hidpi教程](https://www.jianshu.com/p/bcb0f04bfd96)

- [8/9代IntelCpu核显开启HDMI输出](https://blog.daliansky.net/Tutorial-Using-Hackintool-to-open-the-correct-pose-of-the-8th-generation-core-display-HDMI-or-DVI-output.html)

- [B360M核显输出HDMI](https://blog.csdn.net/he37176427/article/details/89670213)

- [黑苹果启动参数问题](https://heipg.cn/drivers/whatevergreen-139.html)

- [黑苹果HDMI接口唤醒黑屏问题](http://bbs.pcbeta.com/viewthread-1850729-1-1.html)
---