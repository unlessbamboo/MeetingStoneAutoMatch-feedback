# MeetingStoneAutoMatch · 反馈与发行

集合石 · 自动匹配版（MeetingStoneAutoMatch）的**发行包与问题反馈**仓库。插件源码不在此仓库公开。

- 适用客户端：时光服 `_classic_titan_`（Interface 38002）、无限服 `_forever_`（Interface 16001）
- 作者：旧迹微光
- 许可：All Rights Reserved（见 [LICENSE](LICENSE)）

## 下载

到 [Releases](https://github.com/unlessbamboo/MeetingStoneAutoMatch-feedback/releases) 下载最新 `MeetingStoneAutoMatch-<版本>.zip`，解压后把顶层 `MeetingStoneAutoMatch/` 放进：

```text
World of Warcraft/_classic_titan_/Interface/AddOns/   # 时光服
World of Warcraft/_forever_/Interface/AddOns/          # 无限服
```

升级、旧目录迁移与存档处理见包内 `UPGRADE.md`。不要同时启用旧版与新版。

## 反馈问题

点 [New issue](https://github.com/unlessbamboo/MeetingStoneAutoMatch-feedback/issues/new/choose) 选「问题反馈 / Bug report」，按表单填写。提交前请先搜索是否已有相同问题。

不会用 GitHub 也可以：在获取本插件的平台项目页留言，作者会转录到这里。

### 怎么取日志

1. 游戏内输入 `/console scriptErrors 1` 打开 Lua 报错显示（已装 BugSack / BugGrabber 可直接用）。报错弹出时**整段截图**，不要只截第一行。
2. 复现一次问题，记下：哪个页签、点了什么、当时是否在队伍里 / 战斗中 / 刚 `/reload`。
3. 复现完立刻输入 `/jjh diag`，等窗口里的环境自检跑完，点底栏「全选复制」，按 `Ctrl+C`，粘贴到 issue；内容长就存成 `report.txt` 拖进输入框。
4. 游戏崩溃或界面打不开时：正常退出游戏，附上
   `WTF/Account/<账号>/SavedVariables/MeetingStoneAutoMatch.lua`
   （时光服在 `_classic_titan_`，无限服在 `_forever_`；文件含角色名，可先删掉无关段落）。
5. 频道相关（收不到活动、申请发不出去）加跑 `/jjh chan`；界面错位加跑 `/jjh uicheck`，并写明哪一页、哪个控件。

报告头部已包含插件版本、客户端 build、interface 号、角色与最近 60 条日志，不需要另抄。

### 标题与隐私

- 标题写清客户端与现象，例如：`[时光服] 地下城页签点「申请」没有反应（0.3.21）`
- 提交前遮挡角色名、服务器、聊天内容、好友列表、账号与支付信息；日志里的错误行不要改写。

## Issues

- 本仓库只处理本插件的使用问题与兼容性问题，不接收整合包 / 其他插件的问题。
- 修复会在后续版本说明里标出版本号；关闭 issue 时会写清在哪个版本修复。
- 功能建议也可以提交，但不保证排期。

---

## English

Download the latest `MeetingStoneAutoMatch-<version>.zip` from [Releases](https://github.com/unlessbamboo/MeetingStoneAutoMatch-feedback/releases) and extract `MeetingStoneAutoMatch/` into your `Interface/AddOns/`. Remove private information (character names, realm, chat, account details) before posting logs or screenshots.

This repository hosts release packages and the issue tracker only; the source is not public. Free to use, All Rights Reserved — see [LICENSE](LICENSE).
