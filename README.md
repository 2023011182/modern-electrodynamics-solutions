# 现代电动力学习题解答 LaTeX 框架

## 目录结构

- `main.tex`：主文件，负责文档结构、目录、附录和参考文献。
- `preamble/packages.tex`：宏包、页边距、页眉、超链接、参考文献设置。
- `preamble/commands.tex`：常用数学命令和题目/解答环境。
- `chapters/chXX.tex`：每章一个文件，每章包含“思考题”和“课后习题”两部分。

## 编译

推荐使用 XeLaTeX：

```powershell
latexmk -xelatex main.tex
```

如果没有 `latexmk`，可以手动运行：

```powershell
xelatex main.tex
xelatex main.tex
```

## 录入题目

每道思考题使用：

```latex
\begin{thinking}{1.1}
  题干：...

  \begin{solution}
    ...
  \end{solution}
\end{thinking}
```

每道课后习题使用：

```latex
\begin{exercise}{1.1}
  题干：...

  \begin{solution}
    ...
  \end{solution}
\end{exercise}
```
