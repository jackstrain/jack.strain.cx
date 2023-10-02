+++
title = 'Zotero Libreoffice Integration No Icons'
date = 2023-10-02T13:23:02+01:00
tags = ['linux', 'ubuntu', 'libreoffice', 'zotero']
draft = false
+++
Having spent half an hour trying to get the Zotero integration in LibreOffice to work (getting LibreOffice to detect Java needed the `libreoffice-java-common` package by the way), the toolbar appeared and worked, but without icons.  

Getting the icons to work required the following:  
First, close LibreOffice.  
Second, run the following commands:  
```
rm -r ~/.config/libreoffice/4/user/temp/
rm -r ~/.config/libreoffice/4/user/extensions/
```  

Now after starting LibreOffice, you should see the icons instead of just words for each button on the Zotero toolbar.  
