# On the Motive Power of Words
[**St. John's College**](https://sjc.edu/)
2018 Freshmen Language paper on the select quotation of *Introductory Lectures on Psycho-Analysis*, by Sigmund Freud.
Written by Shen Zhou Hong [`<shong@sjc.edu>`](mailto:shong@sjc.edu)

## Essay Information
### Essay Prompt

> Pick *only one* of the following quotations and write a **500-600 word** reflection on it: *your* thoughts; no secondary sources  or bibliography. Your paper will be evaluated on your ability to clearly follow these instructions as well as on the clarity of your writing and your thoughts about the nature of language as expressed in the quotations you choose to write about.

***As assigned by Tutor Carl for the Freshman language Paper Assignment, Fall 2018***


### Essay Quotation
> "Words were originally magic and to this day words have retained much of their ancient magical power. By words one person can make another blissfully happy or drive them to despair, by words the teacher conveys his knowledge to his pupils, by words the orator carries his audience with him and determines their judgements and decisions. Words provoke effects and are in general the means of mutual influence among men."

***By Freud, from the Introductory Lectures on Psycho-Analysis***

#### Quotation Analysis
* **"Words were originally magic"**:

* **"By words one person can [affect another person's emotional state]"**:

* **"By words the teacher conveys his knowledge"**:

* **"By words the orator [can affect judgement]"**:

* **"Words [are the means of] mutual influence among men"**:

### Essay Structure Planning


## Technical Information
### Compiling document
In order to compile latex source files, run `make` in the terminal:
```
cd latex
make
make clean
```

Note: for any partial compiles where compilation fails at a certain point, you
should run `make clean` followed by make again. Trying to run make after a
failed compile would result in additional errors.

### Dependencies
This template uses a makefile to compile the latex source files. The makefile
uses `latexmk`, which runs latex the correct number of times. This is because
due to the presense of figures, tables, and biblatex databases, latex needs to
be called multiple times in some cases. Latexmk should be included in your
latex installation, but if it is now, you may download it here:

* http://personal.psu.edu/jcc8//software/latexmk-jcc/

Additionally, this template uses XeLaTeX by default, as it allows the inclusion
of unicode characters in the latex source files. If XeLaTeX is not installed, or
plain LaTeX is required, simply alter the `makefile` at the appropriate call:

```
# MAIN LATEXMK RULE
$(source_name).pdf: $(source_name).tex
  ...
	latexmk -pdf -xelatex -use-make $<
```

XeLaTeX allows one to use foreign characters like ü or æ natively in the latex
source files, though. So it's probably a good idea to install XeLaTeX:

* http://xetex.sourceforge.net/

### Related documentation
For an overview of how to populate biblatex `citations.bib` files, visit the
biblatex-mla manual at CTAN.

* https://www.ctan.org/pkg/biblatex-mla

### GPLv3 License
The raw template itself is licensed under the terms of the GPL (version 3). A
full copy of the license is attached in `LICENSE.md`. Naturally, any works
that you create using this template (i.e. any actual essays you write using
it) will be your own intellectual property. The GPLv3 license only applies to
any derivative templates.
