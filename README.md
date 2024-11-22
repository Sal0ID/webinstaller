# Webinstaller
This library will continue download even if connection drops.
# Contents
- ## [Installation](https://github.com/Sal0ID/webinstaller/edit/main/README.md#installation-1)
- ## Simplest use
- ## Advanced usage
  - Specify destination
  - CLI use
  - Launch file after download
  - Add shortcut to startup folder
 
# Installation
 ```
git clone https://github.com/Sal0ID/webinstaller
cd webinstaller
python setup.py bdist_wheel
pip install dist/webinstaller-0.1.0-py3-none-any.whl
 ```
# Simplest use
1. Upload some random file to google drive right click it Share->Share->Set general access to anyone with the link
2. Create venv or just create python file
```
from webinstaller import webinstaller

drive_url = "insert_link_from_google_drive_here"

webinstaller.download_file_from_google_drive(drive_url)
```
3. Congratulations, you can launch your program!
