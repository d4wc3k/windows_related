1. Enter generic KEY
CGK42-GYN6Y-VD22B-BX98W-J8JXD
slmgr /ipk CGK42-GYN6Y-VD22B-BX98W-J8JXD
#
2) Download universal tickets pack
https://program.box[.]com/s/326odzt3lhkv77m15b17k6dzx6j24cvw
#
3) Now enter below code in PowerShell:
(Get-ItemProperty HKLM:\SYSTEM\CurrentControlSet\Control\ProductOptions).OSProductPfn
This command will you show you some text like Microsoft.Windows.48.X19-98841_8wekyb3d8bbwe
#
4) This command will you show you some text like Microsoft.Windows.48.X19-98841_8wekyb3d8bbwe
You need to find the exact same name ticket file in the folder which you have extracted earlier.
Copy that ticket file and paste it in the following folder:
C:\ProgramData\Microsoft\Windows\ClipSVC\GenuineTicket
#
5) Now run below command in PowerShell to apply the ticket:
clipup -v -o
#
6) Activate Windows with the following command:
slmgr /ato
#
7) Check Activation Status with the following command:
slmgr /xpr
