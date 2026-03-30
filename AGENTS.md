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
├── scripts/        # Git hooks 等脚本
├── Jian/           # Jian 个人资源目录
├── README.md       # 仓库说明
├── AGENTS.md       # AI Agent 协作指南
└── .gitignore      # Git 忽略规则
```

## Agent 行为准则

### 文件操作

1. **创建文件**：遵循现有目录结构，放入正确分类
2. **命名规范**：使用清晰的命名，避免特殊字符
3. **敏感信息**：禁止提交密码、密钥、Token 等敏感数据

### 提交规范

**强制格式**: `type(scope): description`

**示例**: `feat(private-market): viewer context 解析、市场模式 schema 与统一方案文档`

#### 允许的类型

| 类型 | 说明 |
|------|------|
| `feat` | 新功能 |
| `fix` | 修复 bug |
| `docs` | 文档变更 |
| `style` | 代码格式调整 |
| `refactor` | 重构代码 |
| `test` | 测试相关 |
| `chore` | 构建/工具变动 |
| `add` | 新增资源 |
| `update` | 更新资源 |
| `remove` | 删除资源 |
| `perf` | 性能优化 |
| `ci` | CI/CD 配置 |
| `build` | 构建系统 |
| `revert` | 回滚提交 |

#### 格式说明

- `type`: 必填，提交类型
- `scope`: 可选，影响范围/模块名称
- `description`: 必填，简短描述

#### Git Hook 验证

仓库已配置 `commit-msg` hook，不符合规范的提交将被拒绝。

安装 hook（克隆仓库后执行）：

```bash
# 方式一：复制 hook 文件
cp scripts/commit-msg .git/hooks/commit-msg
chmod +x .git/hooks/commit-msg

# 方式二：配置 Git hooks 路径
git config core.hooksPath scripts/
```

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