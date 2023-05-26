# WSL

## Find your distro
```
# open Windows Powershell as Admin

cd C:\Users\<User>\AppData\Local\Microsoft\WindowsApps

ls

# Look for your Linux distro
```

## Change WSL Default User
```
# open Windows Powershell as Admin

cd C:\Users\<User>\AppData\Local\Microsoft\WindowsApps

# eg
<linux distro> config --default-user root
<linux distro> config --default-user <some lesser user you have set up>
```

## Reset forgotten user password
```
# open Windows Powershell as Admin

cd C:\Users\<User>\AppData\Local\Microsoft\WindowsApps

# ensure you run as root
<linux distro> config --default-user root

# Run Distro
.\<linux distro>

~# passwd <user you want to change password for>

~# exit

# Now in Powershell, change default user back to a lesser person
<linux distro> config --default-user <some lesser user you have set up>
```
