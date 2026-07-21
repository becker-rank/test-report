## Changing the number of repeatable pages

The template can automatically generate additional pages for the **Test execution steps** table and the **Referenced attachments and evidence** table.

In the LaTeX source file, change the values on lines 39 and 40:

```latex
\newcommand{\TestExecutionPageCount}{1}
\newcommand{\AttachmentPageCount}{1}
```
