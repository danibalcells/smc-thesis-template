# smc-thesis-template
LaTeX template for SMC Master's Theses

Put together by Daniel Balcells, based on the [UPF PhD Thesis template](https://www.upf.edu/bibtic/guiesiajudes/eines/tesis/a4latex.zip), 
with some personal additions for better visual appeal and functionality.

### Disclaimer
By no means am I a LaTeX expert. This template is the result of adapting a pre-existing template,
using a lot of help from [TeX Stack Exchange](http://tex.stackexchange.com). As a result, there are some elements of the code
whose behavior I do not fully understand and cannot entirely explain or justify. 
Most of the class definition in `0-Misc/smc_thesis.cls` is a mystery to me, although I've added some useful comments to the
main `thesis.tex` file; and tried to make this a minimum working prototype that allows the non-expert LaTeX user to focus on 
writing without having to deal with the LaTeX code too much. If you're comfortable with LaTeX, feel free to mess 
around with the code and try your own variations!

### Organization
- The main file is `thesis.tex`. It contains the structure of the document rather than the content.
- The thesis info (title, author, etc) is in `0-Misc/preamble.tex`. The class definition `smc_thesis.cls` 
and the bibliography style definition `authoryearbrak.cbx` are also in `0-Misc/`.
- Dedication, acknowledgements and abstract are in `0-Frontstuff`.
- Every chapter and appendix should be in a separate folder (i.e. `1-Introduction/` and `99-Appendix1/`), containing
both the TeX file and a subfolder containing figures. Include these files in the `\mainmatter` section of `thesis.txt` e.g.
`\include{1-Introduction/introduction}` (do **not** add the `.tex` extension in the `include` command!).
- Add your references to `references.bib` using [BibTeX format](http://www.bibtex.org/Format/).

Check it out on [ShareLaTeX](https://www.sharelatex.com/project/58e282b5b6c7b9c414cc4b00)!
