# Metasploit空指令模块

空指令(NOP)是一些对程序运行状态不会造成任何实质性影响的空操作或无关操作指令，最典型的空指令就是空操作，在X86 CPU体系架构平台上的操作码是0x90



在渗透攻击构造恶意数据缓冲区时，常常要在真正要执行Shellcode之前添加一段空指令区，这样当触发渗透攻击后触发执行Shellcode时，有一个较大的安全着陆区，从而避免受到内存地址随机化，返回地址计算偏差等原因造成Shellcode执行失败

