# Gantt Chart Template / 甘特图模板

[English](#english) | [中文](#中文)

---

## English

A lightweight, interactive Gantt chart built in a single HTML file — no dependencies, no installation required.

### Features

- **Zero setup** — open `gantt_template.html` in any modern browser and start editing
- **Fully editable inline** — rename tasks, adjust dates, and manage categories without leaving the page
- **Color-coded categories** — assign tasks to categories with customizable colors
- **Print-ready** — exports a clean SVG-based layout optimized for landscape printing
- **Single file** — everything (HTML, CSS, JS) is self-contained in one file

### Usage

1. Download `gantt_template.html`
2. Open it in your browser (Chrome, Firefox, Safari, Edge)
3. Start building your chart:

| Action | How |
|---|---|
| Rename project | Click the project title at the top |
| Edit start/end period | Click the Start / End fields in the header |
| Add a task | Click **+ Add Task** |
| Rename a task | Click directly on the task name |
| Delete a task | Hover over the task row → click **×** |
| Manage categories | Click **⚙ Categories** to add, rename, or remove |
| Change category color | Open **⚙ Categories** → click the color swatch |
| Print / Export | Click **🖨 Print** |

### Customization

To change the default task and category, edit the following section near the bottom of the `<script>` block:

```js
let cats = [
  {id:1, label:'category1', ...PALETTE[0]},
];

let tasks = [
  {id:1, name:'task1', start:'2024-06-27', end:'2025-12-31', cat:1},
];
```

Dates follow the `YYYY-MM-DD` format. Additional palette colors are defined in the `PALETTE` array at the top of the script.

### Requirements

- Any modern browser (no server needed)
- No npm, no build step, no frameworks

### License

This project is licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

You are free to use, modify, and distribute this project, including for commercial purposes, as long as you include the original copyright notice and a copy of the license. You must also clearly state any changes you made to the original.

[↑ 切换到中文](#中文)

---

## 中文

一个轻量、可交互的甘特图，单个 HTML 文件即可运行，无需任何依赖或安装。

### 功能特点

- **零配置** — 用浏览器直接打开 `gantt_template.html` 即可开始使用
- **页面内直接编辑** — 重命名任务、调整日期、管理分类，无需跳转任何页面
- **颜色分类** — 为任务分配分类，支持自定义颜色
- **打印友好** — 导出干净的 SVG 布局，针对横向打印优化
- **单文件** — HTML、CSS、JS 全部内嵌在一个文件中

### 使用方式

1. 下载 `gantt_template.html`
2. 用浏览器打开（Chrome、Firefox、Safari、Edge 均可）
3. 开始编辑：

| 操作 | 方式 |
|---|---|
| 重命名项目 | 点击顶部项目标题 |
| 修改起止时间 | 点击头部的 Start / End 字段 |
| 新增任务 | 点击 **+ Add Task** |
| 重命名任务 | 直接点击任务名称 |
| 删除任务 | 悬停任务行 → 点击 **×** |
| 管理分类 | 点击 **⚙ Categories** 进行新增、重命名或删除 |
| 修改分类颜色 | 打开 **⚙ Categories** → 点击色块 |
| 打印 / 导出 | 点击 **🖨 Print** |

### 自定义默认数据

在文件底部的 `<script>` 中修改以下内容：

```js
let cats = [
  {id:1, label:'category1', ...PALETTE[0]},
];

let tasks = [
  {id:1, name:'task1', start:'2024-06-27', end:'2025-12-31', cat:1},
];
```

日期格式为 `YYYY-MM-DD`。更多颜色可在脚本顶部的 `PALETTE` 数组中定义。

### 环境要求

- 任意现代浏览器（无需服务器）
- 无需 npm、无需构建、无需框架

### 许可证

本项目采用 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) 许可证。

您可以自由使用、修改和分发本项目（包括商业用途），但须保留原始版权声明和许可证副本，并注明对原始内容所做的修改。

[↑ Back to English](#english)
