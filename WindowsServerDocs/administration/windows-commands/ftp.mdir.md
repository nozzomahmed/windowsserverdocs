---
title: ftp mdir
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 90eec45b-558b-4b8d-bbe4-b56d98e1ca70 vhorne
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---
# ftp: mdir

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Displays a directory list of files and subdirectories in a remote directory.   
## Syntax  
```  
mdir <remoteFile>[ ] <LocalFile>  
```  
#### Parameters  

|  Parameter   |                               Description                                |
|--------------|--------------------------------------------------------------------------|
| <remoteFile> |   Specifies the directory or file for which you want to see a listing.   |
| <LocalFile>  | Specifies a local file to store the listing. This parameter is required. |

## Remarks  
- You can use **mdir** to specify multiple files.  
- Specifying *remoteFile*  
  type a hyphen (**-**) to use the current working directory on the remote computer.  
- Specifying a *LocalFile*  
  type a hyphen (**-**) to display the listing on the screen.  
  ## Examples  
  Display a directory listing of **dir1** and **dir2** on the screen  
  ```  
  mdir dir1 dir2 -  
  ```  
  Save the combined directory listing of **dir1** and **dir2** in a local file called **dirlist.txt**  
  ```  
  mdir dir1 dir2 dirlist.txt  
  ```  
  ## Additional References  
- - [Command-Line Syntax Key](command-line-syntax-key.md)  
