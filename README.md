# AutoHotkey Style Guide

## Table of Contents

Section | Guideline
--------|----------
[Functions](#functions) | [Commands](#commands)
[Naming](#naming) | [Variable Names](#variable-names)    [Constant Names](#constant-names)
[Comments](#comments) | [Comment Style](#comment-style)    [Function Comments](#function-comments)
[Formatting](#formatting) | [Line Length](#line-length)    [Spaces vs Tabs](#spaces-vs-tabs)    [Brace Style](#brace-style)

## Functions

### Commands

Prefer to use a function equilavent. If using a command, the command name must be followed by a comma.

## Naming

### Variable Names

* Variable names are all_lowercase_with_underscores.  
* Prefix private class members with "\_".  
* May prefix global variables with "g_".

### Constant Names

Read-only properties are named with a leading "k" followed by mixed case.

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

## Comments

### Comment Style

Use the ;-style syntax only. Use Doxygen comments.

### Function Comments

Every function declaration should have comments immediately preceding it that describe what the function does and how to use it. These comments should be descriptive ("Opens the file") rather than imperative ("Open the file"); the comment describes the function, it does not tell the function what to do. In general, these comments do not describe how the function performs its task. Instead, that should be left to comments in the function definition.

    ; Brief description of the function.
    ;
    ; Detailed description.
    ; May span multiple paragraphs.
    ;
    ; @param arg1 Description of arg1
    ; @param arg2 Description of arg2. May span
    ;        multiple lines.
    ; @return Description of the return value.
    Compare(arg1, arg2)

## Formatting

### Line Length

Each line of text in your code should be at most 80 characters long.

### Spaces vs Tabs

Use only spaces, and indent 2 spaces at a time. Do not use tabs in your code.

### Brace Style

Use [Allman style braces](https://en.wikipedia.org/wiki/Indent_style#Allman_style), which is braces on its own lines.

### Influences

* [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
* [Neovim C Style Guide](https://neovim.io/develop/style-guide.xml)
* [Python PEP 8](https://www.python.org/dev/peps/pep-0008/)
