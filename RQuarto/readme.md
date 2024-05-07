# Using RQuarto

## Pre-requirements
- `rmarkdown` packages
  - Install: `if(!require("rmarkdown")) install.packages("rmarkdown")` 


Install missing packages:
"LaTeX Error: File `ucharcat.sty' not found"
tinytex::parse_packages(text="LaTeX Error: File `ucharcat.sty' not found")



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
