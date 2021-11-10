# `git release`

## Motivation

I like to write release notes in an annotated tag message.
I *want* to be able to write them in Markdown format, so that
they can easily be translated to GitHub release notes. However, there's a
problem stopping me from being able to do this: `#` to `######` are headers
in Markdown, but comments in git messages.

This git extension is a shortcut to

1. Change the comment character to `;`
2. Start `git tag -a <tag name>`
3. Revert back to the previous comment character (or unset it if it wasn't set)

## Usage

```shell
gh release <tag name>
```
