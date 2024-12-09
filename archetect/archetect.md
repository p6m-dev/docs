# Archetect

## Archetect Installation
<details>
    <summary>Expand/Collapse</summary>

Releases
[https://github.com/archetect/archetect/releases](https://github.com/archetect/archetect/releases)

### Prerequisites
- [Git](../git/git.md)

### Windows

#### Use `installer.exe`
It will automatically :
- add archetect to `Path` environment variable
- set `core.longpaths=true` to support Long File Path for Git
- Set registry `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem\LongPathsEnabled` to `1` to enable Long Path Support for Windows

#### Use `zip` archive
- Unzip archive to desired location
- Enable Long Path Support
  - Add path of archetect executable to `Path` environment variable
  - Enable Git with Long File Name Support `git config --global core.longpaths true`
  - Enable Windows OS Long File Name Support, run `register.exe`, set `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem\LongPathsEnabled` to `1`


### Linux/MacOS
#### Via HomeBrew
```sh 
brew tap archetect/archetect
brew install archetect
```
#### Use `tar.gz` archive
- Extract from archive
- Add path of archetect executable to `PATH` variable
</details>


## Usage
### Initialize with `p6m-catalog` catalog
```sh
archetect render git@github.com:p6m-dev/archetect-initializer.archetype.git ~/.archetect/
```

### Version
```sh
archetect --version
```

### Show catalog
```sh
archetect
```

### Pull most recent version of archetypes
```sh
archetect -U
```

### Predefined answers with `-a` option
```sh
archetect -a org-name=ybor -a solution-name=playground
```

### Clear cache
```sh
archetect cache clear
```
Will remove all cached archetypes and catalogs

### Render archetype from local folder
```sh
archetect render /path/to/archetype
```

### Render archetype from remote repository from branch
```sh
archetect render java-spring-boot-grpc-service.archetype.git@main
```

### Switches with `-s` option
```sh
archetect -s debug-context
```
Will display debug information about archetect context for each archetype called