# Stage Léon

Author:
* First Name Last Name <youremail@example.com>, Paris-Saclay University

## Abstract

### Operational long-term management of a salt cavern for industry targeted green H2 production

An abstract to paste

## Recommanded setup

* Local IDE : [VS code](https://code.visualstudio.com/)

    With extensions
    * [LateX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)

* Perl

    For Windows
    * [StrawberryPerl](https://strawberryperl.com/)

* TeX Distribution

    For Windows
    * [MikTex](https://miktex.org/)

## Perl Scripts

`00_Scripts` folder contains perl script usefull to process TeX file. See [Script documentation](./00_Scripts/README.md) for more informations.


## GitHub Workflow

### build.yaml

This workflow is triggered on any changes in `main` branch.

The first job generate a concatenated TeX file and a word count.

The second job generate PDF from the concatenated TeX file.

The workflow can be manually triggered

### diff.yaml

This workflow is triggered on any changes in a branch that is in a pull request for `main` branch.

The first job generate a concatenated TeX file, a word count and a diff TeX file with `main.tex` from `main` branch.

The second job generate PDF from the concatenated new TeX file and the diff Tex file.

The workflow can be manually triggered



