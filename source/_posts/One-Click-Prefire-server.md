---
title: -CS2-预瞄练习插件一键脚本
date: 2024-04-17 14:33:19
tags: [CS2,CSGO,起源2,服务器,预瞄]
categories: 反恐精英2
---
# -CS2-预瞄练习插件一键脚本

## 使用教程

<iframe src="//player.bilibili.com/player.html?aid=1253152296&bvid=BV1zJ4m1p7X2&cid=1508793003&p=1" scrolling="no" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

## 下载地址

### 最新版本：
<a href="OCPrefire2024.4.20.7z">OCPrefire2024.4.20.7z</a>

### 历史版本：
<a href="OCPrefire2024.4.16.7z">OCPrefire2024.4.16.7z</a>
<a href="OCPrefire2024.4.17.7z">OCPrefire2024.4.17.7z</a>
<a href="OCPrefire2024.4.18测试版.7z">OCPrefire2024.4.18测试版.7z</a>

## 更新日志

```
2024.4.20
脚本更新：
  1. 默认使用了UAC管理员身份运行
  2. 新增了steamcmd为基础的独立服务器安装脚本测试版，该脚本比原版复制用法更稳定但是需要下载。
插件更新至(v0.1.27)(插件作者@冷然斯人)
  插件路线更新：de_anubis中路打A
  1. 尝试修复多人同时训练时出现不受控bot的问题；
  2. 插件运行不再依赖sv_cheats，需要noclip等指令的玩家请在CS2服务窗口自行输入sv_cheats 1或其他跑图指令；
  3. 增加了从文件读取默认设置的功能，减少个人玩家每次进服手动调设置的烦恼。可以重命名 default_cfg.json.example 文件为 default_cfg.json，将其中的数值设置成你常用的数值（数值对应的含义同插件菜单中的难度和训练模式选项）该文件在脚本集成的PFServer\doneplugins\csgo\addons\counterstrikesharp\plugins\OpenPrefirePrac目录下，可以提前更改再进行更新；
  4. 优化了 bot 的复活时间，插件响应更迅速。

2024.4.18测试版
脚本更新：脚本改为UAC授权运行

2024.4.17
脚本更新：添加脚本运行环境检测

2024.4.16
脚本发布
```