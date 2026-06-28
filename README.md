# **华为轻量级智能穿戴设备开发skill**

[英文(English)](README-en.md) | **中文**

### **huawei-lite-wearable-dev 技能速览：**

这个技能是面向 **华为轻量级智能穿戴设备（Lite Wearable）** 应用开发的全流程指导工具。本skill的**设计思路**受华为官方指南启发，官方开发文档：[轻量级智能穿戴应用开发](https://developer.huawei.com/consumer/cn/doc/best-practices/bpta-lite-wearable-guide#section8618133925012)

### **开发目的：**

皆在**便于开发者使用AI编程工具开发应用**，**不可用于商业用途**。

### **功能范围：**

功能范围（Pro版本）：

| 维度          | 具体能力                                 |
| :---------- | :----------------------------------- |
| ArkUI JS 框架 | 指导基于 JS 的声明式 UI 开发，包括组件声明、数据绑定、事件处理等 |
| UI 组件       | 覆盖华为穿戴设备常用组件（文本、按钮、列表、弹窗等）的用法与最佳实践   |
| Canvas 绘图   | 支持自定义绘制场景，如表盘、数据可视化等 2D 绘图需求         |
| Chart 图表    | 指导使用穿戴设备内置 Chart 组件渲染折线图、柱状图等数据图表    |
| 传感器 API     | 调用手表上的心率、加速度、陀螺仪等传感器数据的接口对接          |
| 性能优化        | 针对穿戴设备资源受限的特点，提供渲染、内存、功耗等方面的优化策略     |

功能范围（标准版本）：

| 维度    | 具体能力                  |
| :---- | :-------------------- |
| 项目搭建  | 从零创建手表项目，配置基础结构       |
| 页面开发  | HML + CSS + JS 三件套的写法 |
| 传感器调用 | 心率、血氧、步数、加速度等         |
| 设备能力  | 振动、亮度、存储、电池等          |
| 页面路由  | 多页面跳转、参数传递            |
| 性能优化  | 省电、减少卡顿、适配圆形表盘        |
| 打包发布  | 生成安装包、上架应用市场          |

### 标准版和Pro版区别：

Pro版仅在标准版上对来自Github上的开源项目进行了参考

### 参考项目：

升级版本参考了以下两个 GitHub 项目：

### 1. `scriptiot/hm_lite_wearable_demos`

* **地址**：<https://github.com/scriptiot/hm_lite_wearable_demos>
* **定位**：鸿蒙轻量级穿戴应用组件与 API 示例集合
* **参考的 demo 项目**：
  * `music` — 音乐播放器（`@system.audio` API、矩形 960x480 布局、`swiper` 垂直翻页）
  * `airquality` — 空气质量监测（`@system.sensor` 传感器调用、`@system.app` 应用管理、`@system.router` 路由、`i18n` 国际化）
  * `alarm` — 闹钟应用（`@system.app` 应用生命周期）
  * `showcase-canvas-canvas1` / `canvas6` — Canvas 绘图示例（`getContext("2d")`、`fillRect`、`fillStyle`）
  * `showcase-chart-lineChart-index` / `barChart-indexAttr` — Chart 图表组件示例（`<chart type="line/bar">`、`datasets`、`options`）
  * `showcase-animation-index` — 动画示例（`animate` 关键帧动画）

### 2. `yushu-sjtu/harmonyos-watch-gallery-rtos`

* **地址**：<https://github.com/yushu-sjtu/harmonyos-watch-gallery-rtos>
* **定位**：HarmonyOS Watch 相册应用（针对 Watch GT 6 / HarmonyOS 6.0 的 RTOS 轻量级应用）
* **参考内容**：
  * 网格布局模式（`flex-wrap: wrap` 实现 3x3 缩略图网格）
  * 图片懒加载（`if` 条件渲染，仅加载当前页及前后页图片）
  * 垂直 `swiper` 翻页浏览（`vertical="true"` 实现上下滑动切换）
  * 屏幕常亮控制（`brightness.setKeepScreenOn`）
  * 详情页 `router.replace` 传参模式
  * `list.scrollTo()` 列表滚动控制
  * `onswipe` 手势检测
  * `config.json` 完整配置结构（`abilities`、`js`、`distro`、`apiVersion`）

### 开发技术栈：

* 开发工具：DevEco Studio、Claude Code 等支持使用skills的应用或平台
* 语言：JavaScript + ArkUI JS 框架
* 支持设备：运行 LiteOS 的华为穿戴产品

### 许可证：

本项目采用 **Apache-2.0 许可证** ，同时**遵守华为开发者网站的“使用条款”**。

### 意见反馈/问题反馈/侵权：
请提交issue，会在看到issue后第一时间进行回复、处理。
