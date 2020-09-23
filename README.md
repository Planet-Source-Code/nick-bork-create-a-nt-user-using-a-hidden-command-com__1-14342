<div align="center">

## Create a NT User using a hidden command\.com


</div>

### Description

Simply put, quickly add users to your local machine (NT/Win 2000). This code shows you how to create a user and set them as an Administrator.

You can set nearly all the prefrences for adding a user... email me if you need help doing so!
 
### More Info
 
UserName = NewUser

Password


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nick Bork](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nick-bork.md)
**Level**          |Beginner
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nick-bork-create-a-nt-user-using-a-hidden-command-com__1-14342/archive/master.zip)





### Source Code

```
'Arguments to create the user as a LocalUser and a member of the group Users
TheArguments = "NET USER " & UserName & " " & Password & " /add"
Shell TheArguments, vbHide
'Arguments to add the user as a member of the group Administrators
TheArguments = "NET LOCALGROUP Administrators /Add " & UserName
Shell TheArguments, vbHide
```

