# AGENTS.md

<p align="center">
  <strong>AI Agent 协作指南</strong><br>
  本文档为 AI Agent 提供仓库操作指引
</p>

---

## 仓库概述

`EnchantedTreasure` 是魔仙小队的资源共享中心，用于沉淀团队协作资产。

## 目录结构

```
EnchantedTreasure/
├── docs/           # 项目文档、会议纪要、学习资料
├── assets/         # 设计素材、图标、图片资源
├── snippets/       # 代码片段、脚本、配置模板
├── knowledge/      # 技术分享、经验总结、FAQ
├── templates/      # 通用模板、Checklist、流程文档
├── Jian/           # Jian 个人资源目录
├── README.md       # 仓库说明
└── AGENTS.md       # 本文件
```

## Agent 行为准则

### 文件操作

1. **创建文件**：遵循现有目录结构，放入正确分类
2. **命名规范**：使用清晰的命名，避免特殊字符
3. **敏感信息**：禁止提交密码、密钥、Token 等敏感数据

### 提交规范

使用规范化的提交信息格式：

- `Add: 新增资源` - 添加新文件
- `Update: 更新资源` - 更新现有文件
- `Fix: 修正错误` - 修复问题
- `Remove: 删除资源` - 删除文件
- `Refactor: 重构整理` - 重组目录或文件

### 注意事项

- 大文件（>10MB）需提醒用户考虑使用 Git LFS
- 新增目录时同步更新 README.md 的目录结构
- 保持资源索引的时效性

## 常用操作

### 新增文档

```bash
# 文档放入 docs/ 目录
# 命名格式：<类型>-<日期>-<名称>.md
# 示例：会议纪要-20260330-项目启动.md
```

### 新增素材

```bash
# 素材放入 assets/ 对应子目录
# 按类型分类：icons/、images/、templates/
```

### 新增代码片段

```bash
# 代码放入 snippets/ 目录
# 附带简短说明文件
```

---

*本文档由 AI Agent 维护*