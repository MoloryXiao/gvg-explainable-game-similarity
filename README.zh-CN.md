# GVG 可解释游戏相似度数据集 2026

版本：`0.1.0`  
状态：**正式发布包，尚未上传平台**  
数据快照：2026-09-02

## 包含什么

本候选包包含 50 组不重复游戏配对，覆盖 82 款游戏。每一行都提供：

- 稳定游戏 ID、标题和 Steam App ID；
- 中英文“为什么相似”；
- 中英文“关键差异”；
- 中英文偏好选择建议；
- 两端 Steam 官方商店来源 ID 和 URL；
- 核验日期与置信度。

这些注释是 GVG 为了让推荐理由可检查而制作的编辑判断，不是玩家行为真值，也不表示某款游戏客观上更好。

## 文件

- `data/gvg-explainable-game-similarity-v0.1.csv`：50 组已核验配对；
- `data/sources.csv`：去重后的来源 ID、URL 和抓取日期；
- `DATA-DICTIONARY.md`：字段说明；
- `METHODOLOGY.md`：筛选与核验方法；
- `CORRECTIONS.md`：纠错流程；
- `audit/validation-summary.json`：公开质量摘要；
- `SHA256SUMS.json`：两个 CSV 文件的校验值。

## 核验结果

50 条全部在核对两端当前 Steam 官方记录后保守改写。共核验 82 个唯一 Steam App ID 和 100 个关系端点；候选包中没有残留标题/App ID 串线、重复配对、必填字段缺失或来源 URL 缺失。

官方商店资料可以证明游戏身份和所描述的功能，不能证明“哪款质量更高”或“所有玩家更喜欢哪款”；这部分仍明确标为编辑建议。

## 建议引用格式

在获得 DOI 前：

> Miles. (2026). *GVG Explainable Game Similarity Dataset 2026* (Version 0.1.0). https://gamevgame.com/

Zenodo 发布后，把网站地址替换为 DOI。

## 许可

GVG 原创的数据结构与注释采用知识共享署名 4.0 国际许可协议（`CC BY 4.0`），详见 `LICENSE.md`。

## 纠错

发现游戏身份、功能或翻译错误，可通过 <https://gamevgame.com/contact> 或 `support@gamevgame.com` 反馈。请附上 `relation_id` 和证据链接。
