# LaTeX Business Card

![](example.png)

A simple template for a business card with LaTeX. This setup creates one card (rather than a grid of cards on letter paper), for submission to professional printing service. 

Paper size is of common dimension (at least in the US?) but is customizable, as is the margin size.

The image used in my card is an illustration (of me!) by Shayenna Telles.

## About fonts

This document uses the FontAwesome package for little image icons, which works best with pdfLaTeX. PdfLaTeX doesn't have a lot of options for typefaces though. You could set the document up for XeLaTeX (which has more custom font options), but the user would need to do additional work to make the FontAwesome library available to XeLaTeX. See [here](https://tex.stackexchange.com/questions/132888/fontawesome-font-not-found) or [here](https://stackoverflow.com/questions/30677698/xelatex-fontawesome).

This document happens to use Minion Pro, which is pretty but needs to be set up for pdfLaTeX. I did it with the help of some combination of Kieran Healy's [blog post](https://kieranhealy.org/blog/archives/2012/11/10/installing-minion-pro/)  about this and Sebastian Schubert's [FontPro](https://github.com/sebschub/FontPro) scripts. 

The easiest way to make this work for the typical user would be simply to swap out Minion Pro for another typeface. Learn about easy-to-use LaTeX typefaces [here](https://tug.org/FontCatalogue/).

## Chinese support

![](example-cn.png)

The easiest way to input Chinese is to begin with `business-card-horizontal-cn.tex`. You can input Chinese in the document without modifying it, you must use XeLaTeX to compile it.

The another way to input Chinese is to begin with `business-card-horizontal.tex`. Change 'pdflatex' in line 1 into 'xelatex' and use XeLaTeX to compile it.

Notice: The serif font of Chinese example looks different from original version, because the Chinese example was compiled with default serif font instead of Minion Pro(the contributor to Chinese template have no Minion Pro on his computer).

# Other Business Card Templates

I have the vague feeling that I borrowed a lot of this card design from somewhere...but I can't remember where. I'm sorry.

However, if you would like to investigate other business card templates, see

- [Olivier Pieters](https://olivierpieters.be/blog/2017/02/11/designing-a-business-card-in-latex)
- [Overleaf](https://www.overleaf.com/gallery/tagged/business-cards)
- [Andrew Raim](https://andrewraim.github.io/software/latex-business-card)
