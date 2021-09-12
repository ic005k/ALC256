# ALC256
戴尔笔记本ALC256声卡驱动

ALC256声卡在DELL7472等笔记本上比较特殊，特单独生成一个此型号的驱动。

请注意，音频ID为69.

安装：

1.删除之前的AppleALC.kext

2.拷贝ALC256.kext到kexts目录

3.将音频ID改为69（整数）

此驱动根据最新的AppleALC，修改思路来源于此处：https://github.com/ic005k/DELL7472/issues/47 
