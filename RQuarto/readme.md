# Using RQuarto

## Pre-requirements
- `rmarkdown` packages
  - Install: `if(!require("rmarkdown")) install.packages("rmarkdown")` 


Install missing packages:
"LaTeX Error: File `ucharcat.sty' not found"
tinytex::parse_packages(text="LaTeX Error: File `ucharcat.sty' not found")

# Format
- [Quarto - All Formats](https://quarto.org/docs/output-formats/all-formats.html)

## Presentations

### Revealjs
- [Quarto - Revealjs](https://quarto.org/docs/presentations/revealjs/)

## Documents

### HTML 
- [Quarto - HTML Basics](https://quarto.org/docs/output-formats/html-basics.html)

### PDF
- [PDF Basics](https://quarto.org/docs/output-formats/pdf-basics.html)


# Computations
- [Quarto - Using R](https://quarto.org/docs/computations/r.html)
- [Quarto - Execution Options](https://quarto.org/docs/computations/execution-options.html)
- [Quarto - R Inline Code](https://quarto.org/docs/computations/inline-code.html#knitr-2)

# Interactivity
- [Quarto - Interactivity](https://quarto.org/docs/interactive/)

# Theming

## HTML Theming
- [Quarto - HTML Theming](https://quarto.org/docs/output-formats/html-themes.html) (incl. `fontsize`)

## "Draft" watermark on pages/slides

Define the `draft-watermark` css-style:
```
<style>
.draft-watermark {
    position: fixed; top: 50%; left: 50%;
    transform: translate(-50%, -50%) rotate(-45deg);
    z-index: 1000;
    font-size: 100px; font-weight: bold; color: #ccc; opacity: 0.5; }
</style>
```

Use the `draft-watermark` css-style on a page/slide:
```
<div class="draft-watermark">Draft</div>
```
