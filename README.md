# markdown sandbox

This example regex is taken from [GitLab's issue closing pattern](https://docs.gitlab.com/ee/administration/issue_closing_pattern.html)

## String contains regex

'\b((?:[Cc]los(?:e[sd]?|ing)|\b[Ff]ix(?:e[sd]|ing)?|\b[Rr]esolv(?:e[sd]?|ing)|\b[Ii]mplement(?:s|ed|ing)?)(:?) +(?:(?:issues? +)?%{issue_ref}(?:(?:, *| +and +)?)|([A-Z][A-Z0-9_]+-\d+))+)'

## regex in table

|name|value|
|-|-|
|test|'\b((?:[Cc]los(?:e[sd]?|ing)|\b[Ff]ix(?:e[sd]|ing)?|\b[Rr]esolv(?:e[sd]?|ing)|\b[Ii]mplement(?:s|ed|ing)?)(:?) +(?:(?:issues? +)?%{issue_ref}(?:(?:, *| +and +)?)|([A-Z][A-Z0-9_]+-\d+))+)'|

## duplicated headers with same name

A test of how links are generated for duplicate headers. This section violates [MD024/no-duplicate-heading/no-duplicate-header](https://github.com/DavidAnson/markdownlint/blob/v0.25.1/doc/Rules.md#md024) on purpose.  

### section A

This is section A.

#### child section

This is child section of section A.

### Section B

This is section B.

#### child section

This is child section of section B. In GitHub, ID is [child-section-1](#child-section-1)

## Footnotes

Sample from [pandoc documentation](https://pandoc.org/MANUAL.html#extension-footnotes):

Here is a footnote reference,[^1] and another.[^longnote]

[^1]: Here is the footnote.

[^longnote]: Here's one with multiple blocks.

    Subsequent paragraphs are indented to show that they
belong to the previous footnote.

        { some.code }

    The whole paragraph can be indented, or just the first
    line.  In this way, multi-paragraph footnotes work like
    multi-paragraph list items.

This paragraph won't be part of the note, because it
isn't indented.

Here is an inline note.^[Inline notes are easier to write, since
you don't have to pick an identifier and move down to type the
note.]

## `CODE_IN_HEADER`

The header of this section is `CODE_IN_HEADER`. How about the id for this?
