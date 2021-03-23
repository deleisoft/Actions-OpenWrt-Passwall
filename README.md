# OpenWrt18.06-X86-64稳定版云编译项目

## 开始之前

本项目上游firkerword/openwrt-Exclusive，这里修改了部分代码

去除了定时自动编译，有需要的时候手动来编译一次即可，修改了默认后台IP为10.10.10.10，默认密码为password

去除了上传网盘操作，保留了自动发布到Releases，其他未作修改

## 编译说明

在Run Workflow时把SSH connection to Actions的值改为true（或者也可以不修改，而是通过 webhook 方式发送带有ssh触发关键词的请求。）
在触发工作流程后，在 Actions 日志页面等待执行到SSH connection to Actions步骤，会出现类似下面的信息：

ssh Y26QeagDtsPXp2mT6me5cnMRd@nyc1.tmate.io
https://tmate.io/t/Y26QeagDtsPXp2mT6me5cnMRd

复制 SSH 连接命令粘贴到终端内执行，或者复制链接在浏览器中打开使用网页终端。（网页终端可能会遇到黑屏的情况，按 Ctrl+C 即可）

cd openwrt && make menuconfig

完成后按Ctrl+D组合键或执行exit命令退出，后续编译工作将自动进行。

## 固件来源：

P3TERX云编译脚本地址：[https://github.com/P3TERX/Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)

lean固件源码地址：[https://github.com/coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)

由衷感谢所有为openwrt无私奉献的大佬们。

## 固件说明：

lean源码版本，内核为***4.19***版

## 固件下载
### 点击[Actions](https://github.com/deleisoft/openwrt-Exclusive/actions) 或者[Releases](https://github.com/deleisoft/openwrt-Exclusive/releases) 
