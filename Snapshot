##Snapshot Creation

$VMname = get-content C:\Name.txt
$Snapname = get-content C:\snapshotname.txt
get-vm -Name $VMname | New-Snapshot -name $Snapname -Descre $Snapname -Memory:false
Get-Snapshot -vm $VMname | Select-Object VM,Name,create,sizegb,sizemb, | ft | out-file -filepath c:\snapshot-report.txt
