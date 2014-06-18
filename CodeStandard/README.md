#Rocaloid Code Standard

Language: C(with RUtil2)

Version 1, Revision 1

---

1. Preliminaries
---

###1.1 About

This standard instructs collaborators to contribute high-quality codes to Rocaloid, and helps them better understand others' works within Rocaloid Project.

The scope of this standard applies to all **codes written in C** in Rocaloid Project, excluding those in the front end.

###1.2 Definitions

* `Class`: refers to a structure declared by `RClass` of RUtil2.
* `Interface`: refers to anything that collaborators share within the published codes.

2. Format
---

###2.1 File Extension

* Headers should have `.h` file extension.
* RTemplate headers should have `.h` file extension.
* Sources, except RTemplate sources, should have `.c` file extension.
* RTemplate sources should have `.rc` file extension.
* Natural docs documentations should have `.txt` file extension.
* Other markdown-written documents should have `.md` extension.

###2.2 Line

* Tabs should be replaced by space. Tab size should be 4 characters.
* Maximum length for a line is 80 characters.

###2.2.1 Newline and brackets

**Braces** are separated to be in the next line in the following situations:

* After `if`.
* After `else`.
* After `for`.
* After `while`.
* After `do`.
* After `switch`.

And are not separated when:

* Before `else`.
* Before `while` in `do` blocks.

The separated braces should not be indented. But the succedent block should be indented.

###2.3 Spacing

###2.4 Other

3. Namming
---

###3.1 Namespace

###3.2 Variable

###3.3 Function

###3.3.1 Argument

###3.4 Word Choice/Synonyms

* Use `Size` instead of `Length`.

###3.5 Other

4. Interface
---

###4.1 Class

###4.2 Function

###4.2.1 RInterface

###4.3 Macro

###4.4 RTemplate

###4.5 Other

Appendix
---

###I. Examples

###II. Revision History
