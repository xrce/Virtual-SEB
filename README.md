<div align='center'>
    <h1>Installation Guide for Safe Exam Browser in Virtual Machine</h1>
    <br><img height="64" src="https://avatars.githubusercontent.com/u/13450095">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    <img height="64" src="https://cdn-icons-png.flaticon.com/512/2488/2488314.png"><br><br>

```
For educational purpose only
```

</div>

<details>
<summary><font size=3><b>VMWare</b></font></summary>

## Pre-requisites
- [VMWare Workstation](https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html)
- [Windows 10 ISO](https://www.microsoft.com/en-us/software-download/windows10)
- [Safe Exam Browser](https://safeexambrowser.org/download_en.html)
- Text editor

## Setup Virtual Machine

1. Open **VMWare**
2. Create **New Virtual Machine**
3. Select **Typical Configuration**
4. Select **Windows 10 ISO**
5. You can customize configuration for automatic windows installation
6. Enter **Virtual machine name**
7. Leave **Maximum disk size** to default, then select **Split virtual disk into multiple files**
8. You can **Customize Hardware** if you want, make sure you uncheck **Power on this virtual machine after creation**
9. Right click on your machine, then select **Open VM directory**
10. Edit **.vmx** configuration using text editor, then add the below line

    `SMBIOS.reflectHost = "TRUE"`

11. Power on virtual machine, then wait for installation succeeded

## Install Safe Exam Browser

1. Open your virtual machine
2. Install **[Safe Exam Browser](https://safeexambrowser.org/download_en.html) Setup Bundle**

## Patch Safe Exam Browser

1. Download all files from `SafeExamBrowser/Application`
2. Copy and replace downloaded files to `C:\Program Files\SafeExamBrowser\Application`
3. Now you can try to open Safe Exam Browser by clicking on **.seb** file

## What's Working?

- Bypass VM detection
- Live proctoring
- Switch between guest and host machine

## Notes

- Can't use 3.6.0 version, use 3.5.0 instead

</details>
