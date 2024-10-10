# ERC grant LaTeX template

This is a LaTeX template to write ERC research grants.
It was created for the 2025 consolidator grant submission 
and is heavily based on the great work Catrin Campbell-Moore
[here](https://www.overleaf.com/latex/templates/unofficial-erc-template-using-versions/zyqqjfbckwqc).

However, several key things have changed:

- All sections of the template are incorporated in LaTeX
  - CV
  - Funding tables using `tabularx` environment
- Example is shown for split sections B1 and B2, although writing both in one document is still supported.

Some advantages of this template:

- Consistent formatting since everything is written in LaTeX
- Allow to set font to `Adobe Times Roman` for more consistency with original template (use `times` option when loading `ercformatting` package)
- Add instructions of ERC template for guidance (to show, use `showinstructions` option when loading `ercformatting` package)

Details can be found in the individual examples. 
the File `src/b1.tex` also includes,
in addition to the instructions,
some ideas and rationale behind formatting choices.

**Use this template at your own risk.**

## Citation style

We provide three simple citation styles that should lead to clean citations.
They are all BibTeX styles and work with `natbib`.
You can use:

- Author,year type citations with `erc_author_year.bst`
- Numbered citations sorted alphabetically in reference section with `erc_number_alpha.bst`
- Numbered citations sorted in order of appereance in reference section with `erc_number_app.bst`

See the section on the bibliography in the template files.

## Loaded packages

The `ercformatting.sty` file loads a suite of opinionated packages
that should allow you to just start writing. 
Have a look at the top of that file.
Packages that are specified with `\RequirePackage` are necessary for the template to work.
Packages that are specified with `\usepackage` are optional and can be removed if you don't need them
or want to replace them with other, incompatible packages.


## Folder structure

Here is an overview of the important files in this repository:

```
| README.md - This file
| src - Source folder
--| ercformatting.sty - The package that does all the tricks
--| b1.tex - A template for writing part B1
--| b2.tex - A template for writing part B2
| citation_style - Folder with instructions and template to create your own citation styles
--| citation_style.dbj - The driver for creating the `erc_number_app.bst` citation style
--| README.md - Some more info on how to create your own citation style
```

## License

This template is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
