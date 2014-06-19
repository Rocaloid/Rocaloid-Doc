#Rocaloid Code Standard

Language: C(with RUtil2)

Version 1, Revision 0

---

1. Preliminaries
---

###1.1 About

This standard instructs collaborators to contribute high-quality codes to Rocaloid, and helps them better understand others' works within Rocaloid Project.

The scope of this standard applies to all **codes written in C** in Rocaloid Project, excluding those in the front end.

###1.2 Definitions

* `Component`: refers to the source code of a library or executable.
* `User`: refers to anyone who utilize components under Rocaloid Project.
* `Contributor`: refers to anyone who contribute codes to Rocaloid Project.
* `Class`: refers to a structure declared by `RClass` of RUtil2.
* `Interface`: refers to any coding element that contributors share within the published codes.

2. Format
---

###2.1 File Extension

* Headers should have `.h` file extension.
* RTemplate headers should have `.h` file extension.
* Sources, except RTemplate sources, should have `.c` file extension.
* RTemplate sources should have `.rc` file extension.
* Natural docs documentations should have `.txt` file extension.
* Other markdown-written documents should have `.md` file extension.

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

The separated braces **should not** be indented. But the succedent block **should** be indented.

###2.3 Spacing

Additional spacing is required **before and after** these punctuators:

`-> *(as multiply) / + - % << >> < > <= >= == != &(as bitwise AND operator) ^ | && || ? : = *= /= %= += -= <<= >>= &= ^= |=`

Additional spacing is required **before but not after** these punctuators:

`++ --`

Additional spacing is required **after but not before** these punctuators:

`, &(as address operator) ~ ! *(as abstract declarator)`

Additional spacing is **not required** before or after these punctuators:

`. [ ] ( ) { } ; # ## *(as indirection operator)`

###2.3.1 Rule of combination

When **one of** the above rules is satisfied, a space should be inserted before or after the punctuator, except when a space(**including indent**) already exists in the target location.

###2.4 Other

The above rules apply to macro definitions.

3. Naming
---

All C-written codes follow an extended **Upper Camel Case** naming method.

###3.1 External Identifier

`External Identifier`:

*   `{Annoymous Prefix(opt)}{Namespace Abbreviation}_{Library-Scope Identifier}`

`Library-Scope Identifier`:

*   `{Class Identifier}_{Annoymous Prefix(opt)}{Method Identifier}`

*   `{Annoymous Prefix(opt)}{Function Identifier}`

`Class Identifier`:

*   `{Class Name}_{Class Architecture(opt)}_{Class Type(opt)}`

`Method/Function Identifier`:

*   `{Function Name}_{Function Architecture(opt)}_{Function Type(opt)}`

`Function Name`:

*   `{Function Prefix(opt)}{Function Core}{Function Postfix(opt)}`

**Namespace Abbreviation should not be used inside RUtil2.**

###3.1.1 Annoymous Prefix

Annoymous Prefix is used to hide an identifier from programmers, to prevent naming collision.

An Annoymous Prefix can be either

*   `_`: to hide an identifier from users.
*   `__`: to hide an identifier from both users and contributors of the component itself.

###3.1.2 Namespace Abbreviation

The abbreviation of a namespace, usually shorter than 7 characters and upper case(but not compulsively). A namespace can be the name of a component.

Examples:

*   `CDSP2`: abbr. Cybervoice engine Digital Signal Processing library 2
*   `CSVP`: abbr. Cybervoice engine Spectral Voice Processing library
*   `RFNL`: abbr. Rocaloid Fast Numerical Library

###3.1.3 Class Name

The name of a Class.

Examples:

*   `FWindow`: Fast Window generator(see RFNL/src/FWindow/)
*   `STFTIterlyzer`: STFT iterative analyzer(see CVESVP/src/Iterator/_STFTIterlyzer.h)

###3.2 Function Arguments

###3.3 Word Choice/Synonyms

* Use `Size` instead of `Length`.

###3.4 Other

The above rules apply to macro definitions.

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
