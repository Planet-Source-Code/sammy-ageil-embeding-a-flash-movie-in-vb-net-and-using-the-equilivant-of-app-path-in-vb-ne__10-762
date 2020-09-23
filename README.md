<div align="center">

## embeding a flash movie in vb\.net and using the equilivant of app\.path in vb\.net


</div>

### Description

To show how to embed any flash (.swf) movie into any VB.Net application and how to use the equilivant of app.path in VB.Net
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Sammy Ageil](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/sammy-ageil.md)
**Level**          |Beginner
**User Rating**    |3.4 (17 globes from 5 users)
**Compatibility**  |VB\.NET
**Category**       |[Graphics/ Sound](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/graphics-sound__10-15.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/sammy-ageil-embeding-a-flash-movie-in-vb-net-and-using-the-equilivant-of-app-path-in-vb-ne__10-762/archive/master.zip)





### Source Code

<table border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse" bordercolor="#111111" width="100%" id="AutoNumber1">
 <tr>
 <td width="100%"><font color="#008000">'To add a flash movie to any vb.net
 app first you need to add the shockwave flash object most likely if your
 system is updated it will be called flash ocx. once its added create a sub
 to play the movie <br>
 mine is as follow:<br>
 </font></td>
 </tr>
</table>
<table border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse" bordercolor="#111111" width="100%" id="AutoNumber2">
 <tr>
 <td width="50%">Private Sub playflash()<br>
 <br>
                  
 With AxShockwaveFlash1 </td>
 <td width="50%"><font color="#008000">'my control name<br>
 </font></td>
 </tr>
 <tr>
 <td width="50%"> .Stop()</td>
 <td width="50%"><font color="#008000">'make sure you control the running of
 the movie</font></td>
 </tr>
 <tr>
 <td width="50%">..Movie = "C:\Documents and Settings\MySide _<br>
 \My Documents\Visual Studio _ Projects\WindowsApplication8\rose.swf"<br>
                           
 </td>
 <td width="50%"><font color="#008000">'now there are three ways to locate
 the movie<br>
 '(1)<br>
 </font></td>
 </tr>
 <tr>
 <td width="50%"> </td>
 <td width="50%"><font color="#008000">'The file HAS TO BE IN THE BIN
 DIRECTORY<br>
 'or this code with result in an EXCEPTION!<br>
 </font></td>
 </tr>
 <tr>
 <td width="50%">.Movie = String.Concat _(Application.StartupPath, _ "\rose.swf")<br>
 </td>
 <td width="50%"><font color="#008000">'(2)  is like using the App.path
 in VB6, The file HAS TO BE IN THE BIN DIRECTORY as well<br>
 </font></td>
 </tr>
 <tr>
 <td width="50%">.Movie =System.Windows.Forms.Application. _ _StartupPath &
 "\rose.swf"<br>
 </td>
 <td width="50%"><font color="#008000">'(3) my fav of all</font></td>
 </tr>
 <tr>
 <td width="50%"> .playing = True<br>
 End With<br>
 End Sub<br>
 </td>
 <td width="50%"><font color="#008000">'now we get it to play.</font></td>
 </tr>
</table>
you can download this code from
http://ecreationscanada.com/downloads.asp?vb
read the .txt file and you will have it working!
Good luck

