# Fd Cheat Sheat

- [Fd Cheat Sheat](#fd-cheat-sheat)
  - [Basics](#basics)
    - [List all files recursively](#list-all-files-recursively)
    - [Regular expression search](#regular-expression-search)
    - [Glob-based search](#glob-based-search)
    - [Case-sensitive search](#case-sensitive-search)
    - [Case-insensitive search](#case-insensitive-search)
  - [Filter](#filter)
    - [Do not respect ignore files](#do-not-respect-ignore-files)
    - [Filter by file extension](#filter-by-file-extension)
    - [Filter by file type](#filter-by-file-type)
  - [Utility](#utility)
    - [Execute a command for each search result](#execute-a-command-for-each-search-result)
    - [Execute a command with all search results at once](#execute-a-command-with-all-search-results-at-once)
    - [Use a long listing format with ls](#use-a-long-listing-format-with-ls)

## Basics

### List all files recursively

```
fd . [PATH]
```

### Regular expression search

```
fd PATTERN [PATH]
```

### Glob-based search

```
fd -g PATTERN [PATH]
```

### Case-sensitive search

```
fd -s PATTERN [PATH]
```

### Case-insensitive search

```
fd -i PATTERN [PATH]
```

## Filter

### Do not respect ignore files

```
fd --no-ignore [PATTERN [PATH]]
```

### Filter by file extension

```
fd -e EXTENSION [PATTERN [PATH]]
```

### Filter by file type

```
fd -t TYPE [PATTERN [PATH]]
```

## Utility

### Execute a command for each search result

```
fd QUERY -x COMMAND
```

### Execute a command with all search results at once

```
fd QUERY -X COMMAND
```

### Use a long listing format with ls

```
fd -l QUERY
```
