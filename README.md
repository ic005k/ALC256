# ALC256
戴尔笔记本ALC256声卡驱动

ALC256声卡在DELL7472等笔记本上比较特殊，特单独生成一个此型号的驱动，该驱动非常轻巧，不足百K。

这个驱动的最大特点是：只需要ALC256.kext这一个文件就可以了，可删除所有之前和ALC256有关联的所有文件，包括SSDT-ALC256.aml、CodecCommander.kext、VerbStub.kext等等之前围绕ALC256进行驱动相关的文件，睡眠唤醒后耳机也不会出现失灵等现象，总之一切都非常正常。

请注意，音频ID为69.

安装：

1.删除之前的AppleALC.kext

2.拷贝ALC256.kext到kexts目录

3.配置文件Config.plist里面将音频ID改为69（整数）

此驱动根据最新的AppleALC，修改思路来源于此处：https://github.com/ic005k/DELL7472/issues/47  ，对所有的贡献者一并表示感谢！
