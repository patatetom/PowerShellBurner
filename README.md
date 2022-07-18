# PowerShellBurner

[`burn.ps1`](burn.ps1) is a PowerShell script intended to « _burn_ » a raw disk image file on a removable USB drive.

```console
> PowerShell -ExecutionPolicy ByPass -File path\to\burn.ps1 -Image path\to\raw\disk\image.img
```

The disk image file will be requested by PowerShell if it is not provided on the command line.

> [`burn.ps1`](burn.ps1) has been tested with PowerShell version 5.1.18362.1474 (`$Host.Version`) under Windows version 10.0.18363.0 (`[Environment]::OSVersion.Version`).
> <br/><br/>
> [`burn.ps1`](burn.ps1) relies on [`dd-removable.exe`](http://www.chrysocome.net/dd) which is embedded directly in the script in the form of a string variable corresponding to a zip archive encoded in base 64.

---

See also :
- [HDD Raw Copy](https://hddguru.com/software/HDD-Raw-Copy-Tool/)
- [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/)
