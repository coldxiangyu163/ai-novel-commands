# 小说创作指令系统

> 一套完整的网文写作辅助指令，覆盖从构思到成稿的全流程。

## 特性

- **全流程覆盖**：灵感 → 设计 → 大纲 → 写作 → 检查 → 润色
- **多题材支持**：末世、玄幻、都市、历史、游戏、言情等 13+ 题材
- **专业编剧系统**：Blake Snyder 节拍表、三维冲突模型、爆点递进曲线
- **智能记忆**：分层记忆系统，解决长篇同质化问题
- **质量保障**：多维度检查，确保设定一致性

## 快速开始

### 1. 开书三连（推荐）

```bash
/idea-mill 末世 系统      # 灵感发散，生成10个候选方案
/packaging-kit            # 包装生产线（书名/简介/标签）
/init-novel               # 初始化项目
```

### 2. 设计阶段

```bash
/design-world             # 世界观设计
/design-characters        # 人物设计
/design-plot              # 剧情设计（自动生成节拍表+爆点曲线）
```

### 3. 大纲规划

```bash
/plan-volume 1            # 规划第一卷大纲
/design-opening           # 极致开篇设计
/check-structure          # 结构完整性检验
```

### 4. 写作

```bash
# 快速模式
/write-fast 1 1           # 极简快速写作

# 精细模式
/plan-chapter 1 1         # 章节细纲
/write-chapter 1 1        # 按细纲写作

# 批量模式
/auto-write 1 1           # 完整流程写作
/batch-write 1 1-5        # 批量写作
```

### 5. 检查润色

```bash
/check-consistency 1 1-10 # 一致性检查
/review-reader 1 1-10     # 读者视角评审
/polish-chapter 1 1-10    # 批量润色
```

## 命令速查

### 初始化

| 命令 | 说明 |
|------|------|
| `/idea-mill [关键词]` | 新书灵感工厂 |
| `/packaging-kit` | 包装生产线 |
| `/init-novel` | 初始化项目 |
| `/validate-concept` | 创意验证 |

### 设计

| 命令 | 说明 |
|------|------|
| `/design-theme` | 主题设计 |
| `/design-world` | 世界观设计 |
| `/design-characters` | 人物设计 |
| `/design-character-arc [角色]` | 人物内核设计 |
| `/design-antagonist [反派]` | 反派设计 |
| `/design-plot` | 剧情设计 |
| `/design-scene <场景>` | 场景设计 |
| `/design-opening` | 开篇设计 |

### 规划

| 命令 | 说明 |
|------|------|
| `/plan-volume <卷号>` | 卷大纲规划 |
| `/plan-chapter <卷号> <章号>` | 章节细纲 |
| `/check-all-volumes` | 全书检查 |
| `/check-structure` | 结构检验 |

### 写作

| 命令 | 说明 |
|------|------|
| `/write-fast <卷号> <章号>` | 快速写作 |
| `/auto-write <卷号> <章号>` | 完整流程写作 |
| `/write-chapter <卷号> <章号>` | 按细纲写作 |
| `/batch-write <卷号> <起始>-<结束>` | 批量写作 |

### 检查润色

| 命令 | 说明 |
|------|------|
| `/check-consistency <卷号> <范围>` | 一致性检查 |
| `/review-reader <卷号> <范围>` | 读者评审 |
| `/polish-chapter <卷号> <范围>` | 章节润色 |
| `/polish-dialogue <卷号> <范围>` | 对话打磨 |

### 记忆管理

| 命令 | 说明 |
|------|------|
| `/update-status init` | 初始化状态 |
| `/update-status sync <章号>` | 同步状态 |
| `/sync-memory <卷号>` | 归档全书记忆 |

## 项目结构

```
[书名]/
├── AGENTS.md              # 写作规范
├── 小说规划.md            # 总体规划
├── 人物档案/              # 人物相关
├── 世界观/                # 世界观相关
├── 动态状态/              # 短期记忆
├── 全书记忆/              # 长期记忆
├── 卷X-卷名/              # 各卷内容
│   ├── 卷X大纲.md
│   └── 章节/
└── 质量检查/              # 检查报告
```

## 文档

- [写作流程指南](docs/写作流程指南.md) - 根据作品类型选择流程
- [完整文档](docs/完整文档.md) - 详细命令说明和进阶用法

## 支持的题材

**男频**：末世、玄幻、都市、仙侠、科幻、历史、军事、游戏、无限流、系统流、赘婿

**女频**：古代言情、现代言情

**其他**：悬疑、恐怖、种田、轻小说

## 版本

**v2.3.4** - 风格铁律强化

查看 [完整文档](docs/完整文档.md#版本历史) 了解更新历史。

## License

MIT
