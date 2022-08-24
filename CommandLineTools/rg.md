# Ripgrep Cheat Sheet

- [Ripgrep Cheat Sheet](#ripgrep-cheat-sheet)
  - [Basics](#basics)
    - [Regular expression search](#regular-expression-search)
    - [Search without using regular expression search](#search-without-using-regular-expression-search)
    - [Case-sensitive search](#case-sensitive-search)
    - [Case-insensitive search](#case-insensitive-search)
    - [Invert match](#invert-match)
    - [Search for multiple patterns](#search-for-multiple-patterns)
  - [Filter](#filter)
    - [Do not respect ignore files](#do-not-respect-ignore-files)
    - [Filter by a file type](#filter-by-a-file-type)
  - [Utility](#utility)
    - [Follow symbolic links](#follow-symbolic-links)
    - [LIst all available file types](#list-all-available-file-types)
    - [Show only the pathes with at least one match](#show-only-the-pathes-with-at-least-one-match)
    - [Show the pathes and the number of lines that match the given patterns](#show-the-pathes-and-the-number-of-lines-that-match-the-given-patterns)

## Basics

### Regular expression search

```
rg [-e] PATTERN [PATH]
```

### Search without using regular expression search

```
rg -F TEXT [PATH]
```

### Case-sensitive search

```
rg -s PATTERN [PATH]
```

### Case-insensitive search

```
rg -i PATTERN [PATH]
```

### Invert match

```
rg -v PATTERN [PATH]
```

### Search for multiple patterns

```
rg -e PATTERN1 -e PATTERN2 [PATH]
```

## Filter

### Do not respect ignore files

```
rg --no-ignore PATTERN [PATH]
```

### Filter by a file type

```
rg -t EXTENSION PATTERN [PATH]
```

## Utility

### Follow symbolic links

```
rg -L PATTERN [PATH]
```

### LIst all available file types

```
rg --type-list
```

### Show only the pathes with at least one match

```
rg -l PATTERN [PATH]
```

### Show the pathes and the number of lines that match the given patterns

```
rg -c PATTERN [PATH]
```
