## Archetect Installation

Releases
[https://github.com/archetect/archetect/releases](https://github.com/archetect/archetect/releases)

### Prerequisites
- [Git](../git/git_installation.md)

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