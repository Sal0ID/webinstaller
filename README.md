# Webinstaller
This library will continue download even if connection drops.
# Contents
- ## [Installation](https://github.com/Sal0ID/webinstaller#installation-1)
- ## [Simplest use](https://github.com/Sal0ID/webinstaller#simplest-use-1)
- ## [Advanced usage](https://github.com/Sal0ID/webinstaller/blob/main/README.md#advanced-usage-1)
  - [Specify destination](https://github.com/Sal0ID/webinstaller/blob/main/README.md#specify-destination)
  - CLI use
  - Launch file after download
  - Add shortcut to startup folder
 
# Installation
1. Upload some random file to google drive right click it Share->Share->Set general access to anyone with the link
2. Install library with this commands or with pip
 ```
git clone https://github.com/Sal0ID/webinstaller
cd webinstaller
python setup.py bdist_wheel
pip install dist/webinstaller-0.1.0-py3-none-any.whl
 ```
# Simplest use
Create venv or just create python file
```
from webinstaller import webinstaller

drive_url = "insert_link_from_google_drive_here"

webinstaller.download_file_from_google_drive(drive_url)
```
3. Congratulations, you can launch your program!
# Advanced usage
## Specify destination
You can specify the destination folder for downloaded files. If the file is in .zip or .rar format, it will be automatically exported to the destination folder that you provided. You can use relative or absolute path. If destination folder doesn`t exist it will create it.

```
from webinstaller import webinstaller

drive_url = "insert_link_from_google_drive_here"
destination = "amogus" 

webinstaller.download_file_from_google_drive(drive_url, destination = destination) #Will create amogus folder and download file there
```
## CLI usage
