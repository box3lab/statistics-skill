# 神岛数据统计 Skill

<p align="center">
  <img src="https://img.shields.io/badge/Skills-Framework-purple?style=flat-square" alt="Skills Framework">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=flat-square" alt="Python">
  <img src="https://img.shields.io/badge/Platform-macOS%20%7C%20Linux%20%7C%20Windows-lightgrey?style=flat-square" alt="macOS | Linux | Windows">
</p>

## 项目简介

这是一个 **Agent Skills** 项目，提供 `dao3-statistics` skill，用于通过命令行查询神岛平台数据（公开数据 + 需要认证的数据）。

实现特点：

- **纯 Python 内置库**：不依赖第三方包
- **输出 JSON**：适合脚本/管道处理
- **覆盖常用查询**：用户资料、地图详情/评论、关注关系、收藏/最近游玩、消息列表、地图统计/留存/行为等

## 快速开始

使用 OpenClaw 安装：

```bash
clawhub install dao3-statistics
```

安装后即可在支持 Skills 的客户端中直接使用。

## 提问示例

当用户提出以下类似问题时，Agent 会自动使用此技能：

- 查一下用户 83354 的资料
- 我想看地图 100131463 的详情和评论
- 帮我搜一下关键词"test"的地图
- 查看我的收藏列表
- 看看最近玩过的地图
- 查看我的粉丝和好友
- 我想看地图的统计数据
- 查看玩家留存数据
- 看看我的系统消息

即使没有明确提到"神岛"，只要描述的是用户资料、地图信息、关注关系、收藏、消息、统计等诉求，Agent 都会优先使用此技能。

## 系统要求

| 项目     | 说明                                     |
| -------- | ---------------------------------------- |
| 操作系统 | macOS / Linux / Windows                  |
| Python   | Python 3.x                               |
| 网络     | 需要访问 `https://code-api-pc.dao3.fun`  |
| 认证信息 | 部分命令需要 `--token` 与 `--user-agent` |
