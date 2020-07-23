黑苹果 技嘉笔记本 New aero 15 SA

# Hackintosh-New-aero-15-SA
(中英双语-Bilingual in English and Chinese)
已经测试运行 Mac OS :Catalina 15.5 15.6

可参阅我的博客(第一篇) :
My blog:

http://dden.me/index.php/archives/5/

## 我的设备规格
## Specs

```
- Processor: i7-9750H
- Memory: 16GB 2667 MHz Samsung DDR4 (Upgraded, originally was 8GB)
- Panel: LCD FHD 144Hz 1920x1080 IPS
- Graphics: Intel UHD Graphics 630 + NVIDIA GeForce GTX 1660ti
- m.2 NVME SSD Samsung 970 evo plus (500G)
I/O | Ports:
- 3x USB 3.1 Gen1 (Type-A)
- 2x Thunderbolt™ 3 (USB Type-C)
- 1x HDMI
- 1x 3.5mm Headphone/Microphone Combo Jack
- 1x SD Card Reader
- 1x DC-in
- LAN Killer E2600 
- WLAN Killer AX1650x (Intel Ax200)
Misc:
- Internal Speaker
- HD Camera
```
### 如何使用 :
### How to use this repository:
### 仅仅针对于 *OpenCore* 用户
### For OpenCore users

写在前面: 如果你不熟悉或者第一次接触OpenCore或者 Hackintosh 请不要随意使用
**NOTE**: If you are unfamiliar with OpenCore or Hackintosh, don't use it

为OpenCore提供了一个通用配置。考虑该存储库的当前macOS支持版本
EFI/OC:所有必需的OpenCore文件(包含kexts, config，补丁等)
- EFI/Boot:必要的启动文件

/OpenCore/ has a general config for OpenCore. Consider the current supported macOS version of this repository

EFI/OC: All necessary OpenCore files (with kexts, configs, patches, etc.)
EFI/Boot: Has other necessary boot files
详细参考() :
 [English wiki](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/ "OpenCore文档")
 [中文用户参考我在这学到很多:Xin's blog博客](https://blog.xjn819.com/?p=543 "OpenCore中文优秀博客")


## Working

**USB Based Devices**
- [x] All USB ports
- [x] Keyboard 
- [x] Bluetooth 
- [x] LAN 
- [x] WLAN (ax200 驱动 感谢远景论坛 大佬@qcwap2012 [原文链接](http://bbs.pcbeta.com/viewthread-1848662-1-1.html "")
	如果你需要使用,截至目前(也就是大佬完全完成驱动 和控制APP之前)你需要配置kext的info文件 具体请参考以上链接
	you'll need to configure the Kext info file by now (before the driver and controlAPP complecated). See the links above for details
	

**Network**
- [x] Ethernet card
- [x] WiFi + Bluetooth

**Power**
- [x] CPU power management
- [x] Battery indicator	(哥们改了两个小时It took two hours to fix )
- [x] USB PM
- [x] Shutdown/Sleep(maybe?)/Restart
- [x] Saving/Restoring screen brightness on reboot

**Graphics**
- [x] Intel graphics card
- [x] HDMI (with Nvidia GC)

**Misc**
- [x] Sound (internal speakers + mic jack on/off)
- [x] Touchpad
- [x] Thunderbolt hotplug

## Not fully working/Issues

- [ ] Built-in speaker 
	~~当外接耳机(Type-C test,i hava no 3.5mm test)插好后，重启笔记本电脑，内置扬声器可能可用，几率小于50%
	When the type-C test (I Hava No 3.5mm Test) is plugged in and the laptop restarts, the built-in speaker may be available, less than 50% of the time~~
	以上问题仅仅针对我个人,其他使用者(百度贴吧)似乎并没有出现
	The above question is only for me, other users do not seem to appear
	注入 CodecCommander.kext 并且在Mac端运行可解决 alc_fix/对应command文件即可
	
- [ ]  ELAN touchpad
	
	就那B样,大部分手势支持.
	
	that's it. Most gestures work

## Support status:

- MacOS 10.15 	 (Catalina)
- MacOS 10.16 	 (Catalina)
- Ready to test 11	 ( Big Sur)
- **If your notebook mold is similar to mine, it should be able to be modified from my base and used, but I am not responsible for it**
## Special thanks to:

Only show I can contact,
```
	小刘黑苹果专业定制 Xiaoliu Hackintosh Studio 
		He did 90% of the work(except for built-in speaker), I just fix and release.
```
## MarkDown template
[Hackintosh-Aero-15X](https://github.com/zacmks/Hackintosh-Aero-15X/blob/master/README.md "Hackintosh-Aero-15X")
