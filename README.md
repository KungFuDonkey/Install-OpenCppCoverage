# Install-OpenCppCoverage

This is action installs OpenCppCoverage v0.9.9.0 on a Windows Github Action runner. After running this action you can use OpenCppCoverage by running the command "opencppcoverage" in a shell. 

## Features
- use OpenCppCoverage on github actions

## Usage

### Github Actions
Standard usage:
```
on: push
jobs:
  install-opencppcoverage:
    runs-on: windows-latest
    steps:
    - name: opencppcoverage
      uses: KungFuDonkey/Install-OpenCppCoverage@v1
```
Optionally you can define a path where opencppcoverage will be installed. This can be done by adding install-folder to the arguments.
```
on: push
jobs:
  install-opencppcoverage:
    runs-on: windows-latest
    steps:
    - name: opencppcoverage
      uses: KungFuDonkey/Install-OpenCppCoverage@v1
      with:
        install-folder: 'your/path/here'
```
## Author
KungFuDonkey (Sietze Riemersma)

## License
GPL-3.0 License