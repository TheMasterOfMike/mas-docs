---
pagetitle: Office C2R Custom Install
---

# Office C2R Custom Install

------------------------------------------------------------------------

## Notes

-   If the below guide is confusing to you then the simplest option for you is to use [Office C2R Installer](office_c2r_links.html).

-   Retail Office (e.g. O365) has latest feature updates and Volume Office (e.g. ProPlus 2021) don't have latest feature updates. Both can be activated using Ohook activation method.

-   Please note that in the official C2R office custom installation method, there is no ISO or any one-click solution available. Below is the simplest guide to installing the customized office.

-   Russian users needs to follow [this guide](bypass-russian-geoblock.html) to bypass geoblock in Office downloading.

------------------------------------------------------------------------

## Custom Installation Guide

First clear previous installation of Office,

-   Uninstall the office with App and Features option in Windows settings.

-   Run `OfficeScrubber.cmd` file from [Office Scrubber](https://github.com/abbodi1406/WHD/raw/master/scripts/OfficeScrubber_11.7z) by abbodi1406 and select `[R] Remove all Licenses` option. You can skip this step if Office was never installed on the system.

Once done,

-   Download [Office Deployment Tool](https://officecdn.microsoft.com/pr/wsus/setup.exe) (ODT)

-   Copy the downloaded `setup.exe` file to the root of the C drive, i.e. `C:\setup.exe`

-   Goto [config.office.com](https://config.office.com/deploymentsettings)

-   If you want Retail Office then select `Microsoft 365 Apps for enterprise` in the office suites section.

-   If you want Volume Office then select `Office LTSC Professional Plus 2021 - Volume License` (Don't select SPLA version) in the office suites section.

-   You can add Visio and Project apps if you need them. Don't select language that is [not available for Project/Visio](office_c2r_links.html) if you are installing these apps.

-   Customize other things and leave them as default where you don't understand something.

-   Once you go through all the options, click on the export button and it will download a file named `Configuration.xml`

-   Copy the downloaded `Configuration.xml` file to the root of the C drive, i.e. `C:\Configuration.xml`

-   Open the command prompt as admin and run the below commands

    ```         
    cd /d C:\
    setup.exe /configure Configuration.xml
    ```

It will now download and install Office. You can activate it with your preferred method.

------------------------------------------------------------------------

## Alternative Methods

-   [YAOCTRU](https://github.com/abbodi1406/WHD/raw/master/scripts/YAOCTRU_v9.0.zip) (Office Downloader) & [YAOCTRI](https://github.com/abbodi1406/WHD/raw/master/scripts/YAOCTRI_v10.6.zip) (Office Installer)

-   [Office Tool Plus](http://otp.landian.vip/)

------------------------------------------------------------------------

## Need help?

-   Check [here](troubleshoot.html).
