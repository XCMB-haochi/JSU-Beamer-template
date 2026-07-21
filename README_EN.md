# Jiangsu University Beamer Templates

English | [简体中文](README.md)

LaTeX Beamer templates for Jiangsu University, in two styles.

| Style | Folder | Look | Best for |
|-------|--------|------|----------|
| **Classic** | [`classic/`](classic/) | Top navigation, college footer, watermark | Course defenses, routine talks |
| **Modern** | [`modern/`](modern/) | Full-bleed title page, clean body slides | Showcase openings, demos |

## Preview

### Classic

| Title | Content |
|:---:|:---:|
| ![Classic title](classic/gallery/title.png) | ![Classic content](classic/gallery/method.png) |

[More images](classic/gallery/) · [Sample PDF](classic/example.pdf)

### Modern

| Title |
|:---:|
| ![Modern title](modern/gallery/title.png) |

[Sample PDF](modern/example.pdf)

## Quick Start

```bash
cd classic
xelatex example.tex
xelatex example.tex

cd modern
xelatex example.tex
xelatex example.tex
```

**XeLaTeX** is required for Chinese. See each style folder’s README for details.

## Layout

```
.
├── classic/     # nav-bar style
├── modern/      # full-bleed title style
├── LICENSE
└── README.md
```

## Credits

- Classic is adapted from the [NJUSE Beamer Template](https://github.com/EagleBear2002/NJUSE-Beamer-Template).
- Modern is adapted from [SINTEF Presentation](https://www.overleaf.com/latex/templates/sintef-presentation/jhbhdffczpnx) and [college-beamer](https://github.com/liu-qilong/college-beamer).

## License

[MIT License](LICENSE). Please keep the credits above when using the Modern style.

---

**Author**: Xu Yibo  
**Institution**: Jiangsu University  
**Updated**: July 2026
