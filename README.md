# Box for Root config
<h1>快速介绍</h1>
<h2>clash_meta的配置文件 支持box for magisk 使用</h2>
<br>副规则集来源<br>https://github.com/xkww3n/Rules<br><br><br>每天12：00更新</br>
<br>主要ruleset来源<br>https://github.com/Loyalsoldier/clash-rules<br><br> <br>每天6：30更新</br>
<br>Geo数据库来源<br>https://github.com/DustinWin/ruleset_geodata?tab=readme-ov-file<br><br> <br>每天2：00更新</br>
DIY规则在我右上角的DIY规则库里，正在施工中

<<<<<<< HEAD
=======
运行action生成整合了geodata的模块
>>>>>>> cbe43eeda964eacafc7ac3a1eec2a5973d1e1a17

<br>检测DNS泄露情况<br>
<br>https://www.browserscan.net/zh/dns-leak<br>
<p align="center">
    <a href="https://github.com/LIghtJUNction/box_for_magisk_config-bfmc-/blob/master/box/clash/config.yaml">
    <img src="https://github.com/LIghtJUNction/CONFIG_RULE_DIY/actions/workflows/click%20me(config).yml/badge.svg" />
    </a>
    <h1>点击此处立刻跳转至config.yaml</h1>
</p>


# 更新记录
<br>v1.0 可以运行<br>
<br>v2.0 初步解决了DNS泄露问题<br>
<br>v3.0 重新排布拉了一下并且删除多余部分<br>

<br>先刷入模块，然后替换config重启，在管理器中查看和管理<br>

<br>https://www.coolapk.com/feed/56727271?shareKey=NzU4YjA5ZTZlMDhkNjY3ODg0Njc~&shareUid=17845477&shareFrom=com.coolapk.market_14.2.3<br>
<br>
short.weixin.qq.com

dns.weixin.qq.com.cn

long.weixin.qq.com<br>
<br>这三个走代理即可让微信走fcm推送<br>






# 为什么创建这个项目
<br>每次打开手机Gemini语音助手显示你当前地区不支持，让我很烦，官方配置功能又不能满足我的要求。于是我花了一下午开始自己编写，顺便发布出来给有相同需求的人使用，如果你还有什么好点子欢迎提出。规则来自另一个项目

[![ID](https://img.shields.io/badge/id-blue.svg?style=for-the-badge)](docs/index_id.md) [![EN](https://img.shields.io/badge/en-blue.svg?style=for-the-badge)](docs/index_en.md) [![CN](https://img.shields.io/badge/cn-blue.svg?style=for-the-badge)](docs/index_cn.md)

<h1 align="center">
  <img src="https://github.com/LIghtJUNction/box_for_magisk_config-bfmc-/releases/download/v1.0/like.this.jpg" alt="BOX" width="200">
  <br>如图所示，如果自动下载出现问题可以试试<br>
</h1>

<h1 align="center">
  <img src="https://github.com/LIghtJUNction/box_for_magisk_config-bfmc-/releases/download/v2.0/test.jpg" alt="BOX" width="200">
  <br>测试对比结果<br>
</h1>
<h4 align="center">Transparent Proxy for Android(root)</h4>


## Apk Manager
BFR Manager [Download](https://github.com/taamarin/box.manager) optional
> note: notifications will appear continuously, to fix this open Magisk Manager, Click SuperUser, search BoxForRoot, disable logs and notifications 

## Module Directory
MODDIR=/data/adb/box
MODLOG=/data/adb/box/run
SETTINGS=/data/adb/box/settings.ini
> notes: before editing the file **/data/adb/box/settings.ini**, make sure BFR is turned off

## Manage service start / stop
The following core services are collectively referred to as BFR

BFR service is auto-run after system boot up by default.
You can use Magisk/KernelSU Manager App to manage it. Starting the service may take a few seconds, stopping it may take effect immediately.

> notes: if it doesn't work you can use the command:
```bash
# start
su -c /data/adb/box/scripts/box.service start &&  su -c /data/adb/box/scripts/box.iptables enable

# stop
su -c /data/adb/box/scripts/box.iptables disable && su -c /data/adb/box/scripts/box.service stop
```

## Credits
- [CHIZI-0618/box4magisk](https://github.com/CHIZI-0618/box4magisk)
