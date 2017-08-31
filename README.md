# EnvironmentSetup

Steps to run from an elevated powershell cmd prompt:

```Set-ExecutionPolicy Unrestricted```

```. { iwr -useb http://boxstarter.org/bootstrapper.ps1 } | iex; get-boxstarter -Force```

```cinst boxstarter --version 2.9.26 -y```

You will need to restart a new elevated powershell cmd prompt at this point.

*Possibly setup disks at this point?*

```Install-BoxstarterPackage -PackageName https://raw.githubusercontent.com/bcraig83/EnvironmentSetup/master/InitialSetup.txt -DisableReboots```

```Install-BoxstarterPackage -PackageName https://raw.githubusercontent.com/bcraig83/EnvironmentSetup/master/MoveLibraries.txt -DisableReboots```

```Install-BoxstarterPackage -PackageName https://raw.githubusercontent.com/bcraig83/EnvironmentSetup/master/InstallSoftware.txt -DisableReboots```
