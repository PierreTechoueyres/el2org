- [What is el2org](#org70af39d)
  - [Installation](#orge582c1b)
  - [Configure](#orgdc3f7cb)
  - [Usage](#org359d841)


<a id="org70af39d"></a>

# What is el2org

el2org is a simple tool，which can convert a emacs-lisp file to org file. You can write code and document in a elisp file with its help.

Note: el2org.el file may be a good example.


<a id="orge582c1b"></a>

## Installation

1.  Config melpa source, please read: <http://melpa.org/#/getting-started>
2.  M-x package-install RET el2org RET
3.  M-x package-install RET ox-gfm RET

    ox-gfm is needed by \`el2org-generate-readme', if ox-gfm can not be found, ox-md will be used as fallback.


<a id="orgdc3f7cb"></a>

## Configure

    (require 'el2org)
    (require 'ox-gfm)


<a id="org359d841"></a>

## Usage

1.  \`el2org-orgify-if-necessary' can convert an elisp file to org-file.
2.  \`el2org-generate-readme' can generate README.md from elisp's "Commentary" section.