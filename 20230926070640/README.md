# Bash command equivalents for PowerShell

| Linux Command          | PowerShell Equivalent                                   |
|------------------------|--------------------------------------------------------|
| ls                     | Get-ChildItem                                          |
| pwd                    | Get-Location                                           |
| cd                     | Set-Location                                           |
| mkdir                  | New-Item -Type Directory                               |
| rmdir                  | Remove-Item                                            |
| touch                  | New-Item -ItemType File                                |
| rm                     | Remove-Item                                            |
| cp                     | Copy-Item                                              |
| mv                     | Move-Item                                              |
| cat                    | Get-Content                                            |
| more, less             | Get-Content -More                                     |
| head, tail             | Get-Content -TotalCount                               |
| grep                   | Select-String                                          |
| find                   | Get-ChildItem                                          |
| ps                     | Get-Process                                            |
| top, htop              | Use Get-Process and others                            |
| kill                   | Stop-Process                                           |
| chmod                  | Manage permissions via ACLs                           |
| chown                  | Manage ownership via ACLs                            |
| df                     | Get-WmiObject -Class Win32_LogicalDisk                |
| du                     | Get-ChildItem, Measure-Object                         |
| tar                    | Use third-party tools like 7-Zip or Compress-Archive/Expand-Archive |
| wget                   | Invoke-WebRequest                                     |
| ssh                    | SSH support or PowerShell Remoting                    |
| sudo                   | Start-Process, Invoke-Command with -RunAsAdministrator |
| netstat                | Get-NetTCPConnection (or other relevant cmdlets)      |
| sed                    | Select-String or regex in PowerShell                   |
| cut                    | Select-Object and calculated properties in PowerShell |
| tr                     | ForEach-Object with string manipulation                |
| awk                    | Select-Object and calculated properties in PowerShell |
| tcpdump                | Use tcpdump on Linux or similar tools                  |
| tail -f                | Get-Content -Wait                                     |
| telnet                 | Use Telnet client or Test-NetConnection               |
| vim                    | vim text editor (run in terminal)                     |
| zip                    | Use Compress-Archive                                  |
| tmux                   | tmux terminal multiplexer (if installed)              |
| free                   | Get-WmiObject -Class Win32_OperatingSystem            |
| vmstat                 | Use Performance Counters or Get-Counter cmdlet        |
| man                    | Get-Help                                               |
| apropos                | Get-Help or use PowerShell modules                    |
| echo                   | Write-Host or Write-Output                            |
| systemctl start        | Start-Service                                         |
| systemctl stop         | Stop-Service                                          |
| systemctl restart      | Restart-Service                                       |
| ip -br a               | Get-NetIPAddress (for IP addresses)                   |

Tags:
```
#bash #powershell
```

Related:
```
* ChatGPT
```
