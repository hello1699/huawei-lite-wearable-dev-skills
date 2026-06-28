# **Development Skills for Huawei Lite Wearable Devices**

### **huawei-lite-wearable-dev Skill Overview:**

This skill is a full-process guidance tool for application development on **Huawei Lite Wearable devices**. The **design concept** of this skill is inspired by Huawei's official guidelines. Official development documentation: [Lite Wearable Application Development](https://developer.huawei.com/consumer/en/doc/best-practices/bpta-lite-wearable-guide#section8618133925012)

### **Development Purpose:**

It is intended to **facilitate developers in using AI programming tools for application development** and **shall not be used for commercial purposes**.

### **Functional Scope:**

Functional Scope (Pro Version):

| Dimension                | Specific Capabilities                                                                                                                                     |
| :----------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ArkUI JS Framework       | Guides declarative UI development based on JS, including component declaration, data binding, event handling, etc.                                        |
| UI Components            | Covers usage and best practices of common components for Huawei wearable devices (text, buttons, lists, pop-ups, etc.)                                    |
| Canvas Drawing           | Supports custom drawing scenarios, such as 2D drawing needs for watch faces, data visualization, etc.                                                     |
| Chart Components         | Guides the use of built-in Chart components of wearable devices to render data charts such as line charts and bar charts                                  |
| Sensor APIs              | Interface docking for calling sensor data (heart rate, acceleration, gyroscope, etc.) on watches                                                          |
| Performance Optimization | Provides optimization strategies for rendering, memory, power consumption, etc., tailored to the resource-constrained characteristics of wearable devices |

Functional Scope (Standard Version):

| Dimension                | Specific Capabilities                                                |
| :----------------------- | :------------------------------------------------------------------- |
| Project Setup            | Create watch projects from scratch and configure the basic structure |
| Page Development         | Syntax of HML + CSS + JS triad                                       |
| Sensor Calling           | Heart rate, blood oxygen, step count, acceleration, etc.             |
| Device Capabilities      | Vibration, brightness, storage, battery, etc.                        |
| Page Routing             | Multi-page jumping, parameter passing                                |
| Performance Optimization | Power saving, reducing lag, adapting to round watch faces            |
| Packaging & Release      | Generating installation packages, listing on application markets     |

### Differences Between Standard and Pro Versions:

The Pro version only references open-source projects from Github on the basis of the Standard version.

### Reference Projects:

The upgraded version references the following two GitHub projects:

### 1. `scriptiot/hm_lite_wearable_demos`

* **URL**: <https://github.com/scriptiot/hm_lite_wearable_demos>
* **Positioning**: A collection of component and API examples for HarmonyOS Lite Wearable applications
* **Referenced demo projects**:
  * `music` — Music player (`@system.audio` API, rectangular 960x480 layout, `swiper` vertical page turning)
  * `airquality` — Air quality monitoring (`@system.sensor` sensor calling, `@system.app` application management, `@system.router` routing, `i18n` internationalization)
  * `alarm` — Alarm clock application (`@system.app` application lifecycle)
  * `showcase-canvas-canvas1` / `canvas6` — Canvas drawing examples (`getContext("2d")`, `fillRect`, `fillStyle`)
  * `showcase-chart-lineChart-index` / `barChart-indexAttr` — Chart component examples (`<chart type="line/bar">`, `datasets`, `options`)
  * `showcase-animation-index` — Animation examples (`animate` keyframe animation)

### 2. `yushu-sjtu/harmonyos-watch-gallery-rtos`

* **URL**: <https://github.com/yushu-sjtu/harmonyos-watch-gallery-rtos>
* **Positioning**: HarmonyOS Watch Gallery Application (RTOS lightweight application for Watch GT 6 / HarmonyOS 6.0)
* **Referenced content**:
  * Grid layout mode (3x3 thumbnail grid implemented with `flex-wrap: wrap`)
  * Image lazy loading (conditional rendering with `if`, loading only images of the current page and adjacent pages)
  * Vertical `swiper` page turning browsing (vertical page switching implemented with `vertical="true"`)
  * Screen always-on control (`brightness.setKeepScreenOn`)
  * `router.replace` parameter passing mode for detail pages
  * `list.scrollTo()` list scrolling control
  * `onswipe` gesture detection
  * Complete `config.json` configuration structure (`abilities`, `js`, `distro`, `apiVersion`)

### Development Tech Stack:

* Development tools: DevEco Studio, Claude Code and other applications/platforms that support the use of skills
* Languages: JavaScript + ArkUI JS Framework
* Supported devices: Huawei wearable products running LiteOS

### License:

This project is licensed under the **Apache-2.0 License** and also **complies with the "Terms of Use" of Huawei Developer Website**.

### Feedback & Issue Reporting & Copyright Infringement Claims
Please submit an issue. We will respond and resolve it promptly upon receipt.
