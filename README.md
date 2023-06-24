# PSGetFileMetadata

## How to use

### Get-FileDateCode

```powershell
PS> .\scripts\GetFileDateCode.ps1 "C:\myphoto.jpg"
Created:  2018/11/15 19:44:01
Modefied: 2021/12/31 18:22:21
20181115T194401
```

### Get-FileProperties

```powershell
PS> .\scripts\GetFileProperties.ps1 "C:\MyExcelNote.xlsx"
Name                        : MyExcelNote.xlsx
Size                        : 81.1 KB
Item type                   : Microsoft Excel Worksheet
Date modified               : 6/18/2023 9:28 AM
Date created                : 5/1/2023 3:32 PM
Date accessed               : 6/24/2023 6:03 AM
Attributes                  : ALP
Offline status              :
Availability                :
...
..
```

```powershell
PS> .\scripts\GetFileProperties.ps1 -FilePath "C:\MyExcelNote.xlsx" -PropertyNames "Name","Title","Categories"
Name                Title                    Categories
----                -----                    ----------
MyExcelNote.xlsx    My Excel Note 2023       Private; note
```

### Get-FilePropertiesInFolder

```powershell
PS> .\scripts\GetFilesPropertiesInFolder.ps1 "C:\Notes" FilterString ".xls*"
...
..
```
