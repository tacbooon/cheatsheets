# ASDF Cheat Sheet

## Table of Contents

- [ASDF Cheat Sheet](#asdf-cheat-sheet)
  - [Table of Contents](#table-of-contents)
  - [Plugin](#plugin)
    - [Add a plugin](#add-a-plugin)
    - [Remove a plugin](#remove-a-plugin)
    - [List plugins registered on asdf-plugins](#list-plugins-registered-on-asdf-plugins)
    - [List installed plugins](#list-installed-plugins)
  - [Package](#package)
    - [Install a specific version of a package](#install-a-specific-version-of-a-package)
    - [Install the latest stable version of a package](#install-the-latest-stable-version-of-a-package)
    - [Install all the versions listed in the .tool-versions file](#install-all-the-versions-listed-in-the-tool-versions-file)
    - [Remove a specific version of a package](#remove-a-specific-version-of-a-package)
    - [List all versions of a package](#list-all-versions-of-a-package)
    - [List installed versions of a package](#list-installed-versions-of-a-package)
    - [Set the package global version](#set-the-package-global-version)
    - [Set the package global version to the latest](#set-the-package-global-version-to-the-latest)
    - [Set the package local version](#set-the-package-local-version)
    - [Set the package local version to the latest](#set-the-package-local-version-to-the-latest)
    - [Display current version set](#display-current-version-set)
    - [Display the path to an install directory](#display-the-path-to-an-install-directory)
    - [Display the path to an executable](#display-the-path-to-an-executable)
  - [Utilities](#utilities)
    - [Recreate shims](#recreate-shims)
    - [Update asdf itself](#update-asdf-itself)

## Plugin

### Add a plugin

```
asdf plugin add NAME
```

### Remove a plugin

```
asdf plugin remove NAME
```

### List plugins registered on asdf-plugins

```
asdf plugin list all
```

### List installed plugins

```
asdf plugin list
```

## Package

### Install a specific version of a package

```
asdf install NAME VERSION
```

### Install the latest stable version of a package

```
asdf install NAME latest[:VERSION]
```

### Install all the versions listed in the .tool-versions file

```
asdf install
```

### Remove a specific version of a package

```
asdf uninstall NAME VERSION
```

### List all versions of a package

```
asdf list all [NAME]
```

### List installed versions of a package

```
asdf list [NAME]
```

### Set the package global version

```
asdf global NAME VERSION
```

### Set the package global version to the latest

```
asdf global NAME latest[:VERSION]
```

### Set the package local version

```
asdf local NAME VERSION
```

### Set the package local version to the latest

```
asdf local NAME latest[:VERSION]
```

### Display current version set

```
asdf current [NAME]
```

### Display the path to an install directory

```
asdf where NAME [VERSION]
```

### Display the path to an executable

```
asdf which COMMAND
```

## Utilities

### Recreate shims

```
asdf reshim [NAME [VERSION]]
```

### Update asdf itself

```
asdf update
```
