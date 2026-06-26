# Python 自招两小时救急 Slidev

这是一套面向初中自主招生编程准备的 Slidev 课件。目标不是系统讲完 Python，而是围绕学生已经接触过的 P01-P06 基础题型，训练她用“程序员拆题法”应对上机补代码和开放题/面试表达。

## 适用场景

- 学生已经有一点 Python 基础。
- 已经看过 P01-P06 这类基础题：`turtle`、输入输出、公式计算、`if/else`、`elif`、`for range`、累加。
- 只有约两小时辅导时间。
- 需要同时准备上机编程和校园项目类开放题。

## 授课主线

不要把这节课讲成“Python 语法大全”。主线只有一句：

> 输入是什么，怎么算，要不要判断，要不要循环，最后输出什么。

对应到代码模型：

- 输入：`input()`、`int()`、`float()`
- 计算：变量和数学公式
- 判断：`if / else`、`if / elif / else`
- 循环：`for i in range(...)`
- 输出：`print(...)`

对应到开放题表达：

- 二维码入口：解决“怎么进入系统”
- 打卡统计：解决“谁参加了”
- 投票排行：解决“怎么互动”

## 两小时建议流程

1. 0-20 分钟：讲考试边界、补代码四步法、常见扣分点。
2. 20-75 分钟：复盘 P01-P06 六个模型。
3. 75-100 分钟：做公式题、判断题、循环题三类变式。
4. 100-120 分钟：用校园活动打卡系统练一题完整开放题。

## 本地运行

安装依赖：

```bash
npm install
```

启动预览：

```bash
npm run dev
```

默认访问：

```text
http://localhost:3030/
```

构建静态站点：

```bash
npm run build
```

导出 PDF：

```bash
npm run export
```

## Vercel 部署

项目已包含 `vercel.json`：

```json
{
  "buildCommand": "npm run build",
  "outputDirectory": "dist"
}
```

Slidev 的构建产物是 `dist/`，不是 `public/`。如果 Vercel 报 `No Output Directory named "public"`，说明项目设置里还在找默认目录，需要以本仓库的 `vercel.json` 为准，或在 Vercel Project Settings 里把 Output Directory 改为 `dist`。

## 文件结构

```text
.
├── slides.md                 # 课件主体
├── style.css                 # 课件样式
├── assets/slides/            # P01-P06 和 2025 题型背景图片
├── vercel.json               # Vercel 构建输出配置
├── package.json              # Slidev 脚本和依赖
└── docs/superpowers/         # 设计说明和实现计划
```

## 讲课提醒

你不需要把自己定位成 Python 老师。更自然的定位是：用工程师经验带她拆题。

现场可以反复强调：

> 题目再变，也逃不出输入、计算、判断、循环、输出。

开放题则按固定顺序回答：

1. 有什么功能？
2. 怎么推广？
3. 为什么这样设计？
4. 和 Python 基础有什么关系？
5. 对学校有什么价值？

