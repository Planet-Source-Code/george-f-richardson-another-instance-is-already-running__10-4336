<div align="center">

## Another Instance is already running ?


</div>

### Description

This code verifies how many instances of a given process name is running on the machine.
 
### More Info
 
ByVal pstrProcessName as String

True if there is another instance or False is there isn't

none that I now


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[George F Richardson](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/george-f-richardson.md)
**Level**          |Beginner
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |VB\.NET
**Category**       |[Algorithims](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/algorithims__10-29.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/george-f-richardson-another-instance-is-already-running__10-4336/archive/master.zip)





### Source Code

```
Imports System
Imports System.Diagnostics
Imports System.ComponentModel
Public Clas TestClas 'It's wrong because pscode.com doesn't accept the word Clas (with 2 s).
  Public Function prevInstance(ByVal pstrProcessName as string) As Boolean
    Dim lblnRet As Boolean = False
    Dim lintInst As Integer
    lintInst = UBound(Diagnostics.Process.GetProcessesByName(pstrProcessName))
    If lintInst > 0 Then
      lblnRet = True
    End If
    Return lblnRet
  End Function
End Clas
```

