# LaTeX 排版模板

这是根据上传压缩包的 LaTeX 项目结构抽取出的占位符模板。正文内容均已替换为“这是……部分”形式，保留了原项目的主要排版结构：

- 米白页面底色
- 深蓝 / 藏红 / 绛粉主题色
- 彩色章节标题与双线装饰
- 双栏目录
- fancyhdr 页眉
- `problem`、`note`、`solution`、`myproof` 环境
- 分章、分节、多文件组织方式

## 编译方式

建议使用 XeLaTeX：

```bash
xelatex main.tex
biber main
xelatex main.tex
xelatex main.tex
```

如果不需要参考文献，也可以暂时注释 `main.tex` 中的 `\printbibliography` 和 `\addbibresource`。

## 文件结构

```text
main.tex
preambles/math-solutions-template.sty
chapters/titlepage.tex
chapters/99_preface-contrib.tex
chapters/99_preface-overview.tex
chapters/01_template-chapter.tex
chapters/01_template-chapter/section-01.tex
chapters/01_template-chapter/section-02.tex
chapters/01_template-chapter/exercises.tex
bib/references.bib
```
