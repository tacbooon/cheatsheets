# Pacman Cheat Sheet

- [Pacman Cheat Sheet](#pacman-cheat-sheet)
  - [Install](#install)
    - [Upgrade all installed packages](#upgrade-all-installed-packages)
    - [Install packages](#install-packages)
    - [Install package groups](#install-package-groups)
    - [Uninstall packages and their dependencies](#uninstall-packages-and-their-dependencies)
    - [Clean package cache](#clean-package-cache)
  - [Query](#query)
    - [Search for packages in the database](#search-for-packages-in-the-database)
    - [Show information about a local package](#show-information-about-a-local-package)
    - [Show information about a remote package](#show-information-about-a-remote-package)
    - [Show a list of packages explicitly installed](#show-a-list-of-packages-explicitly-installed)
    - [Show a list of packages explictly installed and not required as dependencies](#show-a-list-of-packages-explictly-installed-and-not-required-as-dependencies)
    - [Show a list of packages not required as dependencies](#show-a-list-of-packages-not-required-as-dependencies)
  - [Pactree](#pactree)
    - [Show packages which a given package depend on](#show-packages-which-a-given-package-depend-on)
    - [Show packages which depend on a given package](#show-packages-which-depend-on-a-given-package)

## Install

### Upgrade all installed packages

```
pacman -Syu
```

### Install packages

```
pacman -Syu PACKAGE...
```

### Install package groups

```
pacman --needed -Syu GROUP...
```

### Uninstall packages and their dependencies

```
pacman -Rs __PACKAGES__
```

### Clean package cache

```
pacman -Sc
```

## Query

### Search for packages in the database

```
pacman -Ss KEYWORD...
```

### Show information about a local package

```
pacman -Qii PACKAGE
```

### Show information about a remote package

```
pacman -Sii PACKAGE
```

### Show a list of packages explicitly installed

```
pacman -Qe
```

### Show a list of packages explictly installed and not required as dependencies

```
pacman -Qet
```

### Show a list of packages not required as dependencies

```
pacman -Qdt
```

## Pactree

### Show packages which a given package depend on

```
pacman __PACKAGE__
```

### Show packages which depend on a given package

```
pacman -r __PACKAGE__
```
