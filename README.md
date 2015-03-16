# n2n
编译
---

 - 从 OpenWrt 的 [SDK][S] 编译  

   ```bash
   # 以 ar71xx 平台为例
   tar xjf OpenWrt-SDK-ar71xx-for-linux-x86_64-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2
   cd OpenWrt-SDK-ar71xx-*
   # 获取 Makefile
   git clone https://github.com/aa65535/openwrt-chinadns.git package/chinadns
   # 选择要编译的包 Network -> VPN -> n2n/n2n_v2
   make menuconfig
   # 开始编译
   make package/n2n/compile V=99
   ```
