# 江苏大学 Beamer 模板

[English](README_EN.md) | 简体中文

这是本人在大二上学期的《嵌入式应用开发》这门课期中项目答辩时制作的Beamer幻灯片，基于[南京大学软件学院beamer模板](https://github.com/EagleBear2002/NJUSE-Beamer-Template)修改，有许多不足之处，尤其是配色上暂时还没有好好调整，视觉观感比较一般，欢迎各位参与完善。

江苏大学学术演示文稿 LaTeX Beamer 模板，适用于课程答辩、学术报告、项目展示等场景。

## 模板特点

- 江苏大学官方视觉识别系统
- 清晰的顶部导航栏（含校名logo和校徽）
- 绿色主题配色（江苏大学标准色）
- 支持中英文混排
- 16:9 宽屏比例
- 简洁优雅的页面布局

## 目录结构

```
.
├── jsu.sty                          # 江苏大学Beamer样式文件
├── jsu_resources/                   # 模板资源文件夹
│   ├── jsulogo.pdf                  # 江苏大学校徽
│   ├── jsuname.png                  # 江苏大学校名（中英文）
│   └── jsubackground.pdf            # 背景图片
├── example.tex                      # 示例模板文件
├── JSU-Beamer-UniTrack.tex         # 原始项目示例（可供参考）
└── README.md                        # 本说明文件
```

## 快速开始

### 环境要求

- TeX发行版：TeX Live（推荐）或 MiKTeX
- 编译器：XeLaTeX（必须，支持中文）
- 编辑器：TeXstudio、VS Code + LaTeX Workshop 等

### 编译方法

使用 XeLaTeX 编译（推荐）：

```bash
xelatex example.tex
xelatex example.tex  # 编译两次以生成正确的目录和引用
```

或使用 latexmk 自动编译：

```bash
latexmk -xelatex example.tex
```

### 使用方法

1. **复制示例文件**
   ```bash
   cp example.tex my-presentation.tex
   ```

2. **修改基本信息**

   在 `my-presentation.tex` 中修改以下内容：

   ```latex
   \title{你的演示标题}
   \author[姓名]{
       姓名\ 专业班级\\
       学号：xxxxxxxxxx\\
       {\small \url{https://github.com/your-username}}
   }
   \date{2025年XX月}
   ```

3. **添加内容**

   使用 `\section{}` 创建章节，使用 `\begin{frame}...\end{frame}` 创建幻灯片页面。

4. **编译生成PDF**

   使用 XeLaTeX 编译两次生成最终PDF。

## 常用功能

### 创建标题页

```latex
\begin{frame}
    \titlepage
\end{frame}
```

### 创建目录页

```latex
\begin{frame}
    \frametitle{目录}
    \tableofcontents
\end{frame}
```

### 创建普通页面

```latex
\begin{frame}{页面标题}
    页面内容
\end{frame}
```

### 两栏布局

```latex
\begin{frame}{两栏示例}
    \begin{columns}
    \column{0.5\textwidth}
    左侧内容

    \column{0.5\textwidth}
    右侧内容
    \end{columns}
\end{frame}
```

### 列表

```latex
% 无序列表
\begin{itemize}
    \item 第一项
    \item 第二项
\end{itemize}

% 有序列表
\begin{enumerate}
    \item 第一项
    \item 第二项
\end{enumerate}
```

### 插入图片

```latex
\begin{frame}{图片示例}
    \begin{center}
    \includegraphics[width=0.6\textwidth]{images/example.png}
    \end{center}
\end{frame}
```

### 强调块

```latex
\begin{block}{标题}
    内容
\end{block}

\begin{alertblock}{警告}
    重要内容
\end{alertblock}

\begin{exampleblock}{示例}
    示例内容
\end{exampleblock}
```

## 贡献与反馈

如有问题或改进建议，欢迎提交 Issue 或 Pull Request。

## 许可证

本模板遵循 MIT 许可证，可自由使用和修改。

---

**作者**：通信2402 徐奕博
**学校**：江苏大学
**更新时间**：2025年11月
