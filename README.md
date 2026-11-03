# ChatLuna 角色预设集

本仓库收录了一批用于 [ChatLuna](https://chatluna.chat/) 伪装插件（chatluna-character）的角色预设，基于卢恩伪装插件预设模板整理，可直接搭配 QQ 机器人使用。

## 目录结构

```text
.
├── 标准/       # 标准 XML 回复格式（<status> / <think> / <action> / <output>）
└── 工具调用/   # 工具调用（tool call）回复格式
```

两个目录中的同名文件是同一角色的两种版本，按需选用其一：

| 目录 | 回复格式 | 配置要求 |
| --- | --- | --- |
| `标准/` | 标准 XML 格式 | 关闭 chatluna-character 的「实验性工具调用回复」 |
| `工具调用/` | 工具调用格式 | 开启 chatluna-character 的「实验性工具调用回复」 |

## 预设一览

| 角色 | 出处 | 备注 |
| --- | --- | --- |
| Castorice（遐蝶） | 崩坏：星穹铁道 | |
| Cyrene（昔涟） | 崩坏：星穹铁道 | 含语音 |
| SilverWolf（银狼） | 崩坏：星穹铁道 | 含语音 |
| Sparxie（火花） | 崩坏：星穹铁道 | |
| Columbina（哥伦比娅） | 原神 | |
| Sandrone（桑多涅） | 原神 | |
| 下江小春 | 蔚蓝档案 | |
| 浦和花子 | 蔚蓝档案 | |
| 德蕾琪娜·挽昼 | 绝区零 | |
| 诺姆 | 绝区零 | |
| 锁暝 | 鸣潮 | |
| CHARACTER | —— | 官方预设模板，可在此基础上自建角色 |

## 使用前必改

预设中的以下占位符需要替换为你自己的信息：

| 占位符 | 含义 |
| --- | --- |
| `MASTER` | 主人的昵称 |
| `【记得改这里的ID！括号也要删掉！】` | 对应位置的 QQ 号（Bot 自身、MASTER、群友等） |
| `CHARACTER` | 默认模板中的角色名 |
| `example.com` | 示例链接 |
| 「大部分群友的id及详细信息」 | 群友名单 |

各预设文件头部还写有插件依赖与配置说明，建议先通读再修改。

## 插件依赖

预设中用到的主要插件（按需安装）：

- `chatluna-long-memory`：长期记忆
- `chatluna-forward-msg`：合并转发记录读取与发送（可选）
- `chatluna-plugin-common`：通用工具，含群管功能
- `chatluna-toolbox`：戳一戳、贴表情、撤回消息等
- `chatluna-storage-service`：文件存储，防止图床链接过期
- `emojiluna`：表情包发送
- 语音服务：TTS，需自行寻找合适插件或使用 `media-luna`

可选插件：`chatluna-google-gemini-adapter`（Gemini 模型接入）、`chatluna-multimodal-service`（图像/文件描述）、`chatluna-agent`（Agent 与文件处理能力）。

具体配置方式以各预设头部注释为准。

## 隐私说明

仓库中的预设已移除作者的个人 QQ 号与昵称，统一替换为上述占位符。使用前请填入你自己的信息；填入真实信息后的预设不建议再次公开。

## 致谢

- [ChatLuna](https://chatluna.chat/) 及 chatluna-character 插件
- 卢恩伪装插件预设模板（作者 Cook Sleep）
- ChatLuna 官方交流群及各位群友

角色与世界观版权归各作品及原权利方所有，本仓库仅作角色扮演预设分享之用。
