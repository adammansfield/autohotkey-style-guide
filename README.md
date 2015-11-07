# AutoHotkey Style Guide

## Table of Contents

Section | Guideline
--------|----------
[Naming](#naming) | [Variable Names](variable-names)    [Constant Names](constant-names)
  


## Naming

### Variable Names

Variable names are all lowercase, with underscores between words.

    table_count := 5

### Constant Names

Read-only properties are named with a leading 'k' followed by mixed case.

    kDaysInAWeek[]
    {
      get
      {
        return 7
      }
      set
      {
      }
    }


Influences
----------
* [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
* [Neovim C Style Guide](https://neovim.io/develop/style-guide.xml#Variable_Names)
