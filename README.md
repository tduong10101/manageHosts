# ManageHosts

## Description

Powershell script to edit hosts file in "$($Env:WinDir)\system32\Drivers\etc\hosts"

## Parameters:

```
-add: adding host and ip to hosts file. Required hostname and ip.

-remove: removing host from hosts file. Required hostname.

-list: print out current hosts file.

-hostName: host name to be added or removed.

-ip: ip to be added with the hostName.
```

## Example:

Adding new ip and host entry:

```powershell
manageHosts -add -ip 10.10.10.1 -hostName test.testdomain.com
# OR
manageHosts -add 10.10.10.1 test.testdomain.com
```

Remove host entry:

```powershell
manageHosts -remove -hostName test.testdomain.com
# OR
manageHosts -remove test.testdomain.com
```

Print current content of hosts file:

```powershell
manageHosts -list
```
