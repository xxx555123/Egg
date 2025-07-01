# 🐱 Egg计划工具

一个功能丰富的Android Todo应用，具有AI任务管理、离线语音输入和猫咪主题界面。

## ✨ 核心功能

### 🎤 语音输入
- 支持离线语音识别
- 实时语音转文字显示
- 错误修正和重试机制

### 🤖 AI智能处理
- 自动识别任务类型（工作、学习、运动等）
- 智能标记优先级（高、中、低）
- 自动提取Top3重要任务

### 🐱 猫咪主题
- 可爱的猫咪卡片界面
- 不同任务类型对应不同猫咪图标
- Top3任务金色边框和皇冠标识

### 📱 现代化UI
- 森林主题背景
- 毛玻璃效果卡片
- 流畅的动画效果

### 💾 数据管理
- 本地SQLite数据库存储
- Firebase云端同步（可选）
- 离线优先设计

## 🛠 技术栈

- **语言**: Kotlin
- **UI框架**: Jetpack Compose
- **架构**: MVVM + Repository
- **依赖注入**: Hilt
- **数据库**: Room (SQLite)
- **语音识别**: Android SpeechRecognizer
- **云服务**: Firebase (可选)

## 📋 功能特性

### 任务管理
- ✅ 语音/文字输入任务
- ✅ 自动任务分类和优先级识别
- ✅ Top3重要任务突出显示
- ✅ 任务完成状态管理
- ✅ 任务删除和编辑

### 用户体验
- ✅ 实时语音识别反馈
- ✅ 流畅的动画效果
- ✅ 错误提示和处理
- ✅ 空状态友好提示

### 数据统计
- ✅ 今日完成任务统计
- ✅ Top3任务完成统计
- ✅ 待办任务数量显示

## 🚀 快速开始

### 环境要求
- Android Studio Hedgehog | 2023.1.1 或更高版本
- Android SDK 21+
- Kotlin 2.0.21+

### 安装步骤

1. **克隆项目**
   ```bash
   git clone <repository-url>
   cd Egg
   ```

2. **配置Firebase（可选）**
   - 在 [Firebase Console](https://console.firebase.google.com/) 创建新项目
   - 下载 `google-services.json` 文件
   - 替换 `app/google-services.json` 文件

3. **构建运行**
   ```bash
   ./gradlew build
   ```

4. **在Android Studio中运行**
   - 打开项目
   - 连接Android设备或启动模拟器
   - 点击运行按钮

## 📱 使用说明

### 添加任务
1. **语音输入**: 点击麦克风按钮，说出你的计划
2. **文字输入**: 在输入框中输入任务，支持粘贴多行文本
3. **智能识别**: AI会自动识别任务类型和优先级

### 管理任务
- **完成任务**: 点击任务卡片上的复选框
- **删除任务**: 点击删除图标
- **标记重要**: 点击星星图标将任务标记为Top3

### 查看统计
- 应用顶部显示今日完成、Top3完成和待办任务数量
- Top3任务会以金色边框突出显示

## 🎨 界面设计

### 主题色彩
- **森林绿**: 主背景色
- **猫咪橙**: 强调色
- **毛玻璃白**: 卡片背景
- **金色**: Top3任务标识

### 交互效果
- 语音按钮脉冲动画
- 任务完成缩放效果
- 卡片悬停阴影
- 流畅的页面切换

## 🔧 自定义配置

### 修改主题颜色
编辑 `app/src/main/java/com/example/egg/ui/theme/Color.kt` 文件

### 调整AI识别规则
编辑 `app/src/main/java/com/example/egg/ai/TaskProcessor.kt` 文件

### 添加新的猫咪类型
在 `app/src/main/java/com/example/egg/data/Task.kt` 中的 `CatType` 枚举中添加

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📞 联系方式

如有问题或建议，请通过以下方式联系：
- 提交 GitHub Issue
- 发送邮件至 [your-email@example.com]

---

**🐱 让可爱的猫咪帮助你管理每一天的计划吧！** 