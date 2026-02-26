---
title: -CS2-预瞄练习插件一键脚本
date: 2024-04-17 14:33:19
tags: [CS2,CSGO,起源2,服务器,预瞄]
categories: 反恐精英2
---
# -CS2-预瞄练习插件一键脚本

## 使用教程

<iframe src="//player.bilibili.com/player.html?aid=1253152296&bvid=BV1zJ4m1p7X2&cid=1508793003&p=1" scrolling="no" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

注意：使用脚本更新后，如果之前装过困难BOT参数，会被消除，需要再装一遍

## 下载地址

### 最新版本：

<a href="OCPrefire2024.6.10.7z">OCPrefire2024.6.10.7z</a>

### 历史版本：
<a href="OCPrefire2024.4.16.7z">OCPrefire2024.4.16.7z</a>
<a href="OCPrefire2024.4.17.7z">OCPrefire2024.4.17.7z</a>
<a href="OCPrefire2024.4.18测试版.7z">OCPrefire2024.4.18测试版.7z</a>
<a href="OCPrefire2024.4.20.7z">OCPrefire2024.4.20.7z</a>
<a href="OCPrefire2024.4.26.7z">OCPrefire2024.4.26.7z</a>
<a href="OCPrefire2024.4.27测试版.7z">OCPrefire2024.4.27测试版.7z</a>
<a href="OCPrefire2024.5.1.7z">OCPrefire2024.5.1.7z</a>
<a href="OCPrefire2024.5.2测试版.7z">OCPrefire2024.5.2测试版.7z</a>
<a href="OCPrefire2024.5.16.7z">OCPrefire2024.5.16.7z</a>
<a href="OCPrefire2024.5.25测试版.7z">OCPrefire2024.5.25测试版.7z</a>

### 插件默认设置修改方法：
json示例
```json
{
    // 难度:
    //   0: 100HP不回血
    //   1: 500HP不回血
    //   2: +25hp每个击杀
    //   3: +100hp每个击杀(默认)
    //   4: +500hp每个击杀
    "Difficulty": 0,
    // 练习模式:
    //   0: 随机模式
    //   1: 完整模式
    "TrainingMode": 1,
    // BOT武器:
    //   0: 随机
    //   1: UMP45.
    //   2: AK47.
    //   3: SSG08.
    //   4: AWP.
    "BotWeapon": 2,
    // BOT自瞄:
    //0：CS2的原生机器人行为。它以一致的方式工作，但功能较弱。
    //1：基于CSS的瞄准锁定：机器人总是瞄准玩家的头部。但这可能与 CS2 的原生机器人逻辑冲突，导致机器人在某些情况下没有反应。
    //2：基于行为树的瞄准锁定：困难模式。
    "BotAimLock": 2
}
```

#### 脚本1
前往gamePFS\csgo\addons\counterstrikesharp\plugins\OpenPrefirePrac目录下
按照注释编辑default_cfg.json.example，将其重命名为default_cfg.json后重启服务器即可

#### 脚本2
前往PFServer\steamcmd\server\game\csgo\addons\counterstrikesharp\plugins\OpenPrefirePrac目录下
按照注释编辑default_cfg.json.example，将其重命名为default_cfg.json后重启服务器即可

## 更新日志

```
2024.6.10
插件更新：
  1.更新至v0.1.37，路线更新
    de_vertigo
      A坡进攻
      A小道黄布进攻
      中路到CT
      B坡进攻
  稳定性改进、新增基于行为树的BOT锁头，参见（### 插件默认设置修改方法）部分
  2.CSS更新至V239

2024.5.25测试版
插件更新：
  1.更新至v0.1.34，路线更新
    de_dust2
      CT前压B1
      CT中路前顶
  稳定性改进
  2.CSS更新至V234，适配CS2最近的版本大更新
注意：使用脚本更新后，如果之前装过困难BOT参数，会被消除，需要再装一遍

2024.5.16
插件更新：
  1.更新至v0.1.33，路线更新
    de_nuke
      从黄房进攻 A 包点
      从铁板进攻 B 包点
      匪家侧）匪厅入口
      从连接进攻铁板
      从三楼下回防/进攻 A 区
      从匪家外场到 K1
      从 K1 进攻 B 点
      水塔快提正门
      从正门进攻 A 包点
  修复了多人游戏场景下启用/禁用练习的 bug
  为BOT实现了一个简单的锁头功能
  修复插件默认设置功能,参见（### 插件默认设置修改方法）部分
  2.CSS更新至V233,MM更新至1293
脚本更新：
  1.添加困难BOT参数配置文件安装功能，文件来自：https://github.com/lengran/OpenPrefirePrac/issues/17
  该配置文件强化了BOT的反应
  


2024.5.2测试版
插件更新：
  1.更新至v0.1.30，路线更新
    de_dust2
      进攻B点预瞄
      中路夹B预瞄
    de_inferno
      为3条路线添加路线引导线
  2.添加常驻路线进度提示

脚本更新：
  1.回退了快捷方式连接服务器的方式

2024.5.1
插件更新：
  1.适配2024年5月1日CS2更新，MM更新至1290，CSS更新至228
脚本更新：
  1.更换了快捷方式连接服务器的方式，防止一些无效appid情况
  2.增加了部分文本提示

2024.4.27测试版
插件更新：
  1. 路线更新
    de_anubis
      添加CT推A大
      添加CT推B外
      在水下为B点附近增加2个位置
    de_dust2
      在A大和A小区域增加位置
  2.功能更新
    对于自定义练习配置文件的玩家，现在txt模板文件支持对位置的注释。在bot生成位置行中，第8个词及之后的词被视为注释，并且插件会忽略它们。
    现在!prefire命令支持快捷命令。关于快捷方式的使用，您可以在游戏中键入!prefire help 来查看所有的用法。目前支持以下快捷方式：
    !prefire prac [数字]：开始在选定路线上练习。
    !prefire map [地图名称]：切换到另一张地图。
    !prefire df [1-5]：设置难度。
    !prefire mode [rand/full]：设置训练模式。
    !prefire bw [rand/ump/ak/sct/awp]：为bot设置武器。
    !prefire lang [en/pt/zh]：设置语言。en表示英语，pt表示葡萄牙语，中文选择zh。
    !prefire exit：停止练习。
    现在在选择菜单选项后菜单会自动关闭。
    现在可以通过Bot武器菜单或快捷命令设置Bot的武器选择。
    友情提醒：在CS2中，使用AWP的Bot非常菜。如果您想要最强力的目标，AK和鸟狙可能是您最好的选择。

2024.4.26
插件更新：
  1. 更新CSS至v215
  2. 更新MM至Build1289
  3. 插件默认语言改为中文
脚本更新：
  1. 将脚本重新命名方便运行，具体请看压缩包内文本文档
  2. 新增创建快捷方式方法二和Powershell脚本作为备份

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