# my_answerfile

## Answer Files

Info on Answer files can be found here: [Microsoft Docs on Answer Files](https://learn.microsoft.com/en-us/windows-hardware/manufacture/desktop/update-windows-settings-and-scripts-create-your-own-answer-file-sxs?view=windows-11)

This is a repository to save the answer file I use to automate and streamline my windows installs.
It works both on win10 and win11

### I have added the following tweaks

- **Bypasses Windows 11 System Requirements**:
  - Adds registry entries to bypass TPM, Secure Boot, Storage, CPU, RAM, and Disk checks.

- **Debloats Windows**:
  - Removes preinstalled bloatware apps using PowerShell scripts.
  - Removes legacy apps using PowerShell scripts.

- **Registry Tweaks**:
  - Disables Microsoft Account creation.
  - Disables User Account Control (UAC).
  - Disables lock screen and Windows Spotlight.
  - Customizes Start Menu and Taskbar settings.
  - Disables various Windows features like Cortana, Telemetry, Hibernation, and Location Tracking.
  - Configures Windows Update to only install security updates and delay other updates for 2 years.
  - Disables Windows Error Reporting, Delivery Optimization, and Remote Assistance.
  - Sets various performance and privacy-related registry keys.

- **Runs Custom Scripts**:
  - Executes PowerShell and batch scripts to apply additional tweaks and remove specific applications like Microsoft Edge, OneDrive, and Teams.
  - Loads and unloads the Default User registry hive to apply settings for new users.

- **Service Configurations**:
  - Sets numerous Windows services to manual or disabled to optimize performance.

- **Power Plan**:
  - Enables and sets the Ultimate Performance power plan as active.

- **Miscellaneous**:
  - Creates a desktop shortcut for Chris Titus Windows Utility.
  - Disables IPv6 and Teredo.
  - Disables various scheduled tasks related to telemetry and diagnostics.
  - Enables Dark Mode by default.
  - Aligns the Start Button in Windows 11 to the left by default.

In addition to the tweaks I added to the answer file, it also contains elements and scripts from the following sources:

- Base Answer File generation:
  - [Schneegans Unattend Generator](https://schneegans.de/windows/unattend-generator/)
- Windows Tweaks & Optimizations:
  - [ChrisTitusTech WinUtil](https://github.com/ChrisTitusTech/winutil)
- Various Tweaks:
  - [Tiny11Builder](https://github.com/ntdevlabs/tiny11builder)
  - [Ten Forums](https://www.tenforums.com/)
  - [Eleven Forum](https://www.elevenforum.com/)
  - [Winaero Tweaker](https://winaerotweaker.com/)
- Memtechtips
  - memunattendfile

Chris Titus win utility is installed by the script.

### Usage Instructions

If you want to use my script, there's two ways to do it.
- you can directly add this to the win iso file
- or use anyburn software to edit the iso image to include the answer file