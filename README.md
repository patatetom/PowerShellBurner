# PowerShellBurner

`burn.ps1` is a PowerShell script intended to "burn" a raw image file on a removable USB drive.

```console
> PowerShell -ExecutionPolicy ByPass -File \path\to\burn.ps1 -Image c:\path\to\raw\image.img
```

The image file will be requested by PowerShell if it is not provided on the command line.

> `burn.ps1` relies on `dd-removable.exe` which is embedded directly in the script in the form of a string variable corresponding to a zip archive encoded in base 64.
