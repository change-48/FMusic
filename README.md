# FMusic

一款基于 HarmonyOS 开发的本地音乐播放器，支持插件扩展在线音乐搜索与播放。

## 功能特性

### 核心播放功能
- 本地音乐导入与播放
- 多种播放模式：顺序播放、列表循环、单曲循环、随机播放
- 歌词解析与同步显示（支持 LRC 格式）
- 后台播放支持
- 系统播控中心集成（AVSession）
- 实况窗显示支持

### 歌单管理
- 创建自定义歌单
- 歌曲收藏功能
- 歌曲添加/移除
- 多选批量删除
- 歌单切换与快速导航

### 插件系统
- 支持从网络 URL 安装插件
- 支持从本地代码导入插件
- 插件启用/禁用管理
- WebView 沙箱安全执行
- 并行聚合搜索优化

### 搜索功能
- 多插件并行搜索
- 搜索历史记录
- 在线音乐试听与添加

### 界面特性
- 深色/浅色主题自适应
- 毛玻璃效果背景
- 流畅的动画过渡
- 字母索引快速定位
- 左滑快捷操作菜单

## 技术栈

- **开发语言**: ArkTS
- **目标平台**: HarmonyOS API 22
- **音频框架**: AVPlayer (media.AVPlayer)
- **媒体会话**: AVSession (系统播控中心集成)
- **数据存储**: 关系型数据库 (RdbStore)
- **并发处理**: TaskPool (音频文件并发处理)
- **网络请求**: @kit.NetworkKit
- **插件沙箱**: WebView 隔离执行环境

## 权限说明

| 权限 | 用途 |
|------|------|
| `ohos.permission.INTERNET` | 网络访问（插件下载、在线音乐） |
| `ohos.permission.KEEP_BACKGROUND_RUNNING` | 后台音频播放 |
| `ohos.permission.FILE_ACCESS_PERSIST` | 本地音乐文件访问 |


## 编译运行

1. 使用 DevEco Studio 打开项目
2. 同步项目依赖
3. 连接 HarmonyOS 设备或启动模拟器
4. 点击运行


## 系统要求

- HarmonyOS 5.0 及以上
- API Level 22
- 设备类型：手机

## 开发环境

- DevEco Studio 4.0+
- Node.js 14+
- HarmonyOS SDK API 22

## 许可证

本项目仅供学习交流使用。

## 致谢

- HarmonyOS 官方文档
- 所有插件开发者
