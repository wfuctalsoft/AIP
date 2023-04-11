# What is AIP?
AIP - Automatic Installation Package, it will install files or app almost without you.
AIP is similar to APK in simplicity, all you need - double click and wait, files will install quickly and automatically.
For using AIP, you need AIPmini.

# What is AIPmini?
AIPmini is simple reader for AIP files.
AIP files will not open without AIPmini
### Where I can download AIPmini?
You can download it from that repository

# How to create AIP using AIPmini?
Move all your files to one directory (main directory)

![Your directory may look like this](https://github.com/wfuctalsoft/AIP/blob/images/image.png?raw=true)
Create file `Package.aini` in the main directory.
Open it with your text editor.
### Settings for Package.aini
For change manufacturer, add this line in `Package.aini`
```
Manufacturer = -type here what you want (up to 80 chars)-
```
To change description, add this line.
```
Description = -type here what you want (up to 799 chars)-
```
To add EULA, add this line.
> If EULA not needed, don't add this line
```
Eula = -type here what you want (up to 799 chars)-
```
To set shortcut path, add this line.
```
Link = -the name of your file relative to the main directory (up to 128 chars)-
```
If no shortcut needed, add.
```
Link = None
```
Your `Package.aini` may look like this
```
Manufacturer = Ivan Bebrovich
Description = This is some description!
Eula = This is license agreement!
Link = file1.txt
```
### Packing main directory to AIP
Open AIPmini directory with terminal and write this.
```
AIPmini "C:\main directory" to "C:\package.aip"
```
This will pack main directory on disk C: to package.aip on disk C:.
