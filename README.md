# Active Directory Related

## Get AD User Group Membership
```
(Get-ADUser (read-host "User name") -properties memberof).memberof -replace '^CN=([^,]+).+$','$1'
```
