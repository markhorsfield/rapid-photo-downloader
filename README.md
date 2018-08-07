# rapid-photo-downloader
Modified install script for [Rapid Photo Downloader](http://www.damonlynch.net/rapid/index.html)
to allow installation into Python virtual invironments.

[Compare with original version 0.2.0](https://github.com/palto42/rapid-photo-downloader/compare/3264ea48092d738cd5db16a4039dbcf104809d17...master)

## Examples
### Virtual environment using system site packages
Create virtuall environment with
```
mkdir /path/to/virtual/environment
python3 -m venv --system-site-packages /path/to/virtual/environment
source /path/to/virtual/environment/bin/activate
```
Install Rapid Photo downloader
```
python rapid_photo_down_install.py --virtual-env
```

### Virtual environment without system site packages

Create virtuall environment with
```
mkdir /path/to/virtual/environment
python3 -m venv /path/to/virtual/environment
source /path/to/virtual/environment/bin/activate
```
Install Rapid Photo downloader
```
python rapid_photo_down_install.py --virtual-env --user-only
```
#### Run Rapid Photo downloader
`/path/to/virtual/environment/bin/rapid-photo-downloader`

### Uninstall
The script doesn't support uninstall options for virtual environment, but this should not be an issue.
Since it was installed in a venv, the easy way to uninstall it is to just delete the venv folder.
```
rm -r /path/to/virtual/environment
```
