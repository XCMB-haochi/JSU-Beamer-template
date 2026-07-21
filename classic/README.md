# Classic 风格

顶部导航栏、页脚学院信息与校徽水印。适合课程答辩、常规学术报告。

样式参考 [南京大学软件学院 Beamer 模板](https://github.com/EagleBear2002/NJUSE-Beamer-Template)，按江苏大学视觉规范调整。

## 预览

| 封面 | 内容页 |
|:---:|:---:|
| ![封面](gallery/title.png) | ![内容](gallery/method.png) |

完整示例：[example.pdf](example.pdf)

## 编译

```bash
cd classic
xelatex example.tex
xelatex example.tex
```

需要 **XeLaTeX**。

## 使用方法

1. 复制 `example.tex` 为你的文稿。
2. 修改 `\title`、`\author`、`\date`。
3. 用 `\section{}` 划分章节，用 `\begin{frame}...\end{frame}` 写幻灯片。

## 目录说明

```
classic/
├── jsu.sty              # 样式
├── jsu_resources/       # 校徽、校名、水印
├── example.tex          # 示例文稿
├── example.pdf
└── gallery/             # 效果图
```
