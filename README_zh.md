# 🍬 Jelly Garden 三消游戏

<div align="center">

**语言 / Language:** [English](README.md) | [中文](README_zh.md) | [日本語](README_ja.md)

![Unity](https://img.shields.io/badge/Unity-2019.4+-black?style=flat-square&logo=unity)
![C#](https://img.shields.io/badge/C%23-8.0-blue?style=flat-square&logo=c-sharp)
![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20Android-lightgrey?style=flat-square)

完整的三消益智游戏模板，具备现代化功能、社交集成和变现系统。

[功能特性](#-功能特性) • [快速开始](#-快速开始) • [项目结构](#-项目结构) • [文档](#-文档) • [支持](#-支持)

</div>

---

## 📋 目录

- [概述](#-概述)
- [功能特性](#-功能特性)
- [快速开始](#-快速开始)
- [项目结构](#-项目结构)
- [核心系统](#-核心系统)
- [集成与服务](#-集成与服务)
- [文档](#-文档)
- [系统要求](#-系统要求)
- [构建与部署](#-构建与部署)
- [贡献](#-贡献)
- [支持](#-支持)
- [许可证](#-许可证)

---

## 🎮 概述

**Jelly Garden 三消游戏**是一个功能丰富的 Unity 益智游戏模板，专为移动平台设计。以可扩展性和可定制性为核心，包含了启动商业三消游戏所需的一切，从关卡设计工具到变现系统。

### 核心亮点

- 🎯 **完整的三消机制**：经典的交换匹配玩法，包含特殊道具和增强器
- 🗺️ **智能关卡系统**：高级关卡编辑器，包含 100+ 预制关卡
- 💰 **变现就绪**：内购、广告集成和虚拟货币系统
- 🌐 **社交功能**：Facebook 集成、排行榜和好友系统
- 📱 **跨平台支持**：iOS 和 Android 支持，性能优化
- 🎨 **精美 UI/UX**：精美动画、粒子效果和响应式设计

---

## ✨ 功能特性

### 核心玩法

- **三消机制**

  - 经典交换匹配玩法
  - 特殊道具：炸弹、横向/纵向条纹、彩虹道具
  - 连击系统与视觉效果
  - 多种游戏模式和目标

- **关卡系统**

  - 100+ 独特预设计关卡
  - 渐进式难度曲线
  - 星级评分系统（1-3 星）
  - 多种关卡目标（分数、收集、障碍物等）

- **增强器与道具**
  - 游戏前增强器
  - 游戏中增强器
  - 每日奖励系统
  - 生命值系统及自动恢复

### 技术特性

- **关卡编辑器**

  - 可视化关卡设计器
  - 拖放式界面
  - 实时预览
  - 导入/导出功能

- **智能地图系统**

  - 可滚动关卡地图
  - 解锁进度
  - 可视化关卡状态指示器
  - 章节系统

- **动画系统**
  - 流畅的道具转换
  - 匹配粒子效果
  - 屏幕震动效果
  - 奖励动画

### 变现功能

- **应用内购买**

  - 金币包
  - 增强器套装
  - 生命值购买
  - 移除广告选项

- **广告集成**

  - 激励视频广告
  - 插屏广告
  - 横幅广告
  - 广告事件系统

- **虚拟经济**
  - 软货币（金币）
  - 购买追踪
  - 奖励分配

### 社交与网络

- **Facebook 集成**

  - 登录系统
  - 好友列表
  - 头像加载
  - 分数分享

- **排行榜**

  - 全球排名
  - 好友排名
  - 离线支持
  - 分数同步

- **云服务**
  - GameSparks 集成
  - PlayFab 集成
  - 数据持久化
  - 跨设备同步

---

## 🚀 快速开始

### 前置要求

- **Unity**：2019.4 LTS 或更高版本（推荐 2020.3+）
- **操作系统**：Windows 10/11 或 macOS 10.14+
- **IDE**：Visual Studio 2019+ 或 JetBrains Rider
- **移动 SDK**：
  - Android：SDK API Level 19+
  - iOS：Xcode 12+

### 安装步骤

1. **克隆仓库**

   ```bash
   git clone https://github.com/NewbieAudioKid/example-jelly-garden-match-3-unity-5.3.4.git
   cd example-jelly-garden-match-3-unity-5.3.4
   ```

2. **在 Unity 中打开**

   - 启动 Unity Hub
   - 点击"添加"并选择项目文件夹
   - 使用 Unity 2019.4 或更高版本打开
   - 等待项目初始化和包导入

3. **初始设置**

   - 导航到 `Assets/JellyGarden/Scenes/`
   - 打开 `game.unity` 场景进行游戏
   - 打开 `map.unity` 场景进行关卡选择

4. **测试游戏**
   - 点击 Unity 编辑器中的播放按钮
   - 或为目标平台构建

### 快速配置

**基础设置** (`InitScript.cs`)：

```csharp
// 游戏配置
public int startLife = 5;           // 起始生命值
public int startCoins = 100;        // 起始金币
public int levelToOpenEditor = 10;  // 解锁编辑器的关卡
```

**关卡配置**：

- 关卡存储位置：`Assets/JellyGarden/Resources/Levels/`
- 使用内置关卡编辑器编辑关卡
- 访问方式：Unity 菜单 → Window → Level Editor

---

## 📁 项目结构

```
Jelly Garden Match 3/
│
├── Assets/
│   └── JellyGarden/
│       ├── Animation/          # 动画剪辑和控制器
│       │   ├── Item animations
│       │   ├── UI animations
│       │   └── Effect animations
│       │
│       ├── Audio/              # 音效和音乐
│       │   ├── BGM/
│       │   └── SFX/
│       │
│       ├── Fonts/              # 自定义字体和材质
│       │
│       ├── Materials/          # 粒子和着色器材质
│       │
│       ├── Prefabs/            # 可重用游戏对象
│       │
│       ├── Resources/          # 运行时可加载资源
│       │   ├── Levels/        # 关卡数据文件 (.txt)
│       │   ├── Items/         # 三消道具
│       │   └── UI/            # UI 预制件
│       │
│       ├── Scenes/             # Unity 场景
│       │   ├── game.unity     # 主游戏场景
│       │   └── map.unity      # 关卡选择场景
│       │
│       ├── Scripts/            # C# 源代码
│       │   ├── System/        # 核心游戏系统
│       │   ├── GUI/           # UI 控制器
│       │   ├── Integrations/  # 第三方服务
│       │   ├── Leadboard/     # 排行榜系统
│       │   └── Editor/        # Unity 编辑器扩展
│       │
│       ├── SmartLevelsMap/     # 关卡地图系统
│       │
│       ├── Textures/           # 精灵图和图像
│       │   ├── Items/
│       │   ├── UI/
│       │   └── Backgrounds/
│       │
│       └── Documentation/       # PDF 和指南
│
├── ProjectSettings/            # Unity 项目设置
├── Packages/                   # 包依赖
└── README.md                   # 本文件
```

---

## 🔧 核心系统

### 游戏管理器 (`InitScript.cs`)

管理游戏状态、初始化和核心游戏循环的中心枢纽。

**主要职责：**

- 游戏初始化和设置
- 关卡加载和管理
- 玩家数据持久化
- 分数和目标追踪
- 游戏状态管理（游戏中、暂停、完成）

**重要方法：**

```csharp
InitGame()              // 初始化游戏系统
LoadLevel(int num)      // 加载指定关卡
CheckWinLose()         // 检查游戏完成条件
SaveMapPlayerPrefs()   // 保存玩家进度
```

### 匹配系统 (`CombineManager.cs`)

处理所有匹配检测、道具组合和特殊道具生成。

**功能：**

- 三消及以上检测
- 特殊道具创建规则
- 连击链式反应
- 匹配计分系统

### 关卡管理器 (`LevelManager.cs`)

管理关卡数据、目标和进度。

**组件：**

- 关卡数据解析器
- 目标追踪
- 星级计算
- 关卡完成逻辑

### 道具系统 (`Item.cs`, `Square.cs`)

控制单个游戏棋子和棋盘方格。

**道具类型：**

- 简单道具（6 种颜色）
- 条纹道具（横向/纵向）
- 炸弹
- 彩虹道具
- 包裹道具

---

## 🌐 集成与服务

### Facebook 集成

**设置步骤：**

1. 在 [developers.facebook.com](https://developers.facebook.com) 创建 Facebook 应用
2. 将 App ID 添加到 `FacebookManager.cs`
3. 配置 Android/iOS 平台设置
4. 启用所需权限（public_profile、user_friends）

**功能：**

- 用户认证
- 好友列表获取
- 头像加载
- 分数发布

### 广告服务

**支持的网络：**

- Unity Ads
- AdMob
- 自定义广告网络集成

**配置：**

- 编辑 `AdsEvents.cs` 进行广告位置设置
- 为每个平台设置广告单元 ID
- 配置奖励值

### 云后端

**GameSparks 集成：**

- 位置：`Assets/JellyGarden/Scripts/Integrations/Network/Gamesparks/`
- 功能：玩家数据、排行榜、成就

**PlayFab 集成：**

- 位置：`Assets/JellyGarden/Scripts/Integrations/Network/PlayFab/`
- 功能：玩家账户、虚拟经济、统计数据

---

## 📖 文档

项目包含全面的文档：

- **主文档**：`Assets/JellyGarden/JellyGardenDocumentation1.6.pdf`
- **在线指南**：`Assets/JellyGarden/JellyGarden online doc.pdf`

### 文档主题：

1. **入门指南**

   - 项目概述
   - Unity 设置
   - 场景结构

2. **关卡设计**

   - 使用关卡编辑器
   - 创建新关卡
   - 关卡平衡技巧

3. **自定义**

   - 更改视觉效果
   - 修改游戏参数
   - 添加新道具类型

4. **集成指南**

   - Facebook 设置
   - 广告网络集成
   - 后端服务配置

5. **构建与发布**
   - iOS 构建流程
   - Android 构建流程
   - 应用商店提交

---

## 💻 系统要求

### Unity 要求

| 组件       | 最低要求   | 推荐配置    |
| ---------- | ---------- | ----------- |
| Unity 版本 | 2019.4 LTS | 2020.3 LTS+ |
| .NET 版本  | 4.x        | 4.x         |
| 脚本后端   | IL2CPP     | IL2CPP      |

### 平台要求

**iOS：**

- iOS 10.0+
- Xcode 12+
- CocoaPods（用于依赖）

**Android：**

- Android 4.4+（API Level 19）
- Android SDK
- Gradle 6.1.1+

### 硬件要求（开发环境）

- **处理器**：Intel Core i5 / AMD Ryzen 5 或更好
- **内存**：8GB 最低，推荐 16GB
- **存储**：10GB 可用空间
- **显卡**：支持 DirectX 11/12 的 GPU

---

## 🏗️ 构建与部署

### Android 构建

1. **配置播放器设置**

   ```
   File → Build Settings → Android → Player Settings
   - 设置公司名称
   - 设置产品名称
   - 设置包名（com.yourcompany.jellygarden）
   - 设置版本和 Bundle Version Code
   ```

2. **配置密钥库**

   ```
   Publishing Settings
   - 创建或选择密钥库
   - 输入密钥库密码
   - 选择别名和密码
   ```

3. **构建 APK/AAB**
   ```
   File → Build Settings → Android
   - 选择"Build App Bundle (Google Play)"或"Build APK"
   - 选择输出位置
   - 点击 Build
   ```

### iOS 构建

1. **配置播放器设置**

   ```
   File → Build Settings → iOS → Player Settings
   - 设置 Bundle Identifier
   - 设置版本
   - 设置目标 SDK
   - 配置签名
   ```

2. **构建 Xcode 项目**

   ```
   File → Build Settings → iOS
   - 点击 Build
   - 选择输出文件夹
   - 等待 Xcode 项目生成
   ```

3. **在 Xcode 中打开**
   - 打开生成的 .xcodeproj
   - 配置签名证书
   - 为 App Store 构建和归档

### 优化技巧

- **减小构建大小**：

  - 启用代码剥离
  - 使用资源压缩
  - 移除未使用的资源

- **性能优化**：
  - 启用 GPU 实例化
  - 使用纹理图集
  - 优化粒子效果
  - 使用 Unity Profiler 进行性能分析

---

## 🤝 贡献

欢迎贡献！请遵循以下指南：

### 开发工作流程

1. **Fork 仓库**
2. **创建功能分支**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **进行更改**

   - 遵循 C# 编码规范
   - 为复杂逻辑添加注释
   - 必要时更新文档

4. **提交更改**

   ```bash
   git commit -m "添加精彩功能"
   ```

5. **推送到分支**

   ```bash
   git push origin feature/amazing-feature
   ```

6. **打开 Pull Request**

### 代码标准

- 遵循 [Microsoft C# 编码规范](https://docs.microsoft.com/zh-cn/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)
- 使用有意义的变量和方法名
- 为公共 API 添加 XML 文档注释
- 保持方法专注，尽可能在 50 行以内

### 测试

- 提交 PR 前在 iOS 和 Android 上测试
- 确保现有功能无回归
- 使用不同屏幕分辨率测试

---

## 💬 支持

### 获取帮助

- **文档**：查看 `Assets/JellyGarden/` 中的 PDF 指南
- **Issues**：在 GitHub 上提交详细描述的问题
- **邮箱**：support@yourcompany.com

### 报告 Bug

报告 bug 时，请包含：

- Unity 版本
- 平台（iOS/Android/编辑器）
- 重现步骤
- 预期与实际行为
- 截图/日志（如适用）

### 功能请求

我们欢迎功能建议！请：

- 首先检查现有 issues
- 提供清晰的用例
- 描述预期行为
- 考虑实现复杂度

---

## 📄 许可证

本项目为专有软件。保留所有权利。

**使用条款：**

- 允许教育和个人使用
- 商业使用需要许可证
- 未经许可禁止重新分发
- 不提供保证

许可咨询请联系：license@yourcompany.com

---

## 🎯 路线图

### 即将推出的功能

- [ ] 新游戏模式（限时模式、解谜模式）
- [ ] 额外的特殊道具
- [ ] 季节性活动系统
- [ ] 公会/团队系统
- [ ] 聊天功能
- [ ] 实时运营仪表板

### 版本历史

- **v1.6**（当前）

  - 增强的关卡编辑器
  - 性能改进
  - Bug 修复和稳定性

- **v1.5**

  - 添加 PlayFab 集成
  - 新增强器类型
  - UI 改进

- **v1.0**
  - 初始版本
  - 100 个关卡
  - 基础社交功能

---

## 🌟 致谢

### 开发团队

- **首席开发**：[您的名字]
- **游戏设计**：[设计师名字]
- **美术与动画**：[美术师名字]
- **音效设计**：[音效设计师]

### 第三方资源

- **UI 框架**：Unity UI
- **粒子效果**：自定义效果
- **音频**：授权音乐和音效
- **字体**：Boris Black Bloxx、Candy Script

### 特别感谢

感谢所有贡献者和 Unity 社区的支持与反馈！

---

## 📞 联系方式

**项目维护者**：[您的名字]

- GitHub：[@NewbieAudioKid](https://github.com/NewbieAudioKid)
- 邮箱：contact@yourcompany.com
- 网站：[yourcompany.com](https://yourcompany.com)

---

<div align="center">

**使用 Unity 精心打造**

[⬆ 返回顶部](#-jelly-garden-三消游戏)

</div>

