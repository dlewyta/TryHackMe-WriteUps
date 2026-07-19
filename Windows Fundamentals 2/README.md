# TryHackMe - Windows Fundamentals 2

## System Configuration and Advaned System Settings
### System Configuration
- MSConfig is used for advanced troubleshooting
- The main purpose of MSConfig is to help diagnose startup issues
- The system configuration utility has 5 tabs:
  1. General
  2. Boot
  3. Services
  4. Startup
  5. Tools
 
#### General
- we can select what devices and services for windows to load upon boot
- the options are: Normal, Diagnostic or Selective

#### Boot
- Allows us to define various boot options for the OS

#### Services
- lists all servies configured for the system regardless of their state (running or stopped)
- services are special applications that run in the background

#### Startup
- you can access the startup folder by pressing **Win + R**, which opens the Run Dialog
- Then type **shell:startup** and press Enter
- this displays all startup programs as shortcuts or executables

### Advanced System Settings
- additional configuration settings to control performance behaviour and system recovery are found in **view advanced system settings** in the search bar
- windows uses a page file as extra virtual memory space when physical RAM is full
- under **startup and recovery** in the **advanced** tab, you can create a crash dump file
- a crash dump file allows the admin or analysts to understand what went wrong during the crash

## Change UAC Settings
- there are four levels/categories of UAC settings:
  1. Always Notify: windows notifies you when any apps or you try to make any changes to desktop dims
  2. Notify for Apps: Windows notifies you whenever apps try to make changes but not you (the default setting)
  3. same as Notify for Apps, but the screen does not dim
  4. Never Notify: Windows doesn't notify you ever

- You can find the current level by looking in the **User Account Control Settings** window

## Computer Management
- use **compmgmt** to access the Computer Management panel
#### System Tools
- view scehduled tasks by clicking on **Task Scheduler Library**
- Event viewer lets us view events that have occured on the computer
- There are 5 types of events that can be logged:
  1. Error
  2. Warning
  3. Information
  4. Success Audit
  5. Failure Audit

#### Storage
- Can find options for **Windows Server Backup** and **Disk Management**

#### Services and Applications
- allows you to click on different services and see their names, status, etc
- additional detail found in **properties** (right-click)

## System Information
- the System Information (msinfo32) tool gathers information about your computer and displays a comprehensive view of your hardware, system components, and software environments
- Msinfo32 can be used to diagnore computer issues
- the **system summary** section is divided into 3 parts: Hardware Resources, Components, Software Environment

### Components
- shows specific information about the hardware devices installed on the computer

### Software Environment
- you can see information about software baked into the OS and software you have installed

## Resource Monitor
- Resource Monitor displays information about CPU, memory, disk, and netword usage
- has four sections:
  1. CPU
  2. Disk
  3. Network
  4. Memory

## Command Prompt
- the **hostname** command will output the computer name
- the **whoami** command will output the name of the logged in user
- the **ipconfig** command shows the network address settings for the computer (you can use **ipconfig/all** for detailed information)
- the **netstat** command displays protocol status and current TCP/IP network connections
- the **net** command supports sub-commands and is used to manage network resources
- use a command followed by /? for a manual page **EX: ipconfig /?**

## Answers to Questions
### Task 2
1. What is the name of the service that lists Systems Internals as the manufacturerer?
   **A: PsShutdown**
   EXPLANATION: Found in the Services tab of **System Configuration**
2. Whom is the Windows license registered to?
   **A: Windows User**
   EXPLANATION: search bar-> msconfig -> tools -> About Windows -> Launch -> Windows User (at the bottom)
3. What is the command for Windows Troubleshooting
   **A: C:\Windows\System32\control.exe /name Microsoft.Troubleshooting**
   EXPLANATION: search bar -> msconfig -> tools -> Windows Troubleshooting -> command
4. What command will open the control Panel? (the .exe not the full path)
   **A: control.exe**
   EXPLANATION: N/A

### Task 3
1. What is the command to open User Account Control Settings? (The .exe not the path)
   **A: UserAccountControlSettings.exe**
   EXPLANATION: search bar -> msconfig -> tools -> Change UAC Settings -> the last part in the command (piece with .exe)

### Task 4
1. What is the command to open Computer Management? (.msc, not path)
   **A: compmgmt.msc**
   EXPLANATION: found in the system config tools tab
2. When is the npcapwatchdog scheduled task set to run at?
   **A: at system startup**
   EXPLANATION: search bar -> compmgmt -> task scheduler -> active tasks -> npcapwatchdog
3. What is the name of the hidden folder that is shared?
   **A: sh4r3dF0ld3r**
   EXPLANATION: compmgmt -> system tools -> shared folders -> shares -> sh4r3dF0ld3r

### Task 5
1. What is the command to open System Information? (.exe not full path)
   **A: msinfo32.exe**
   EXPLANATION: N/A
2. What is listed under System Name?
   **A: THM-WINFUN2**
   EXPLANATION: search bar -> msinfo32 -> system summary
3. Under Environment Variables, what is the value for ComSpec?
   **A: %SystemRoot%\system32\cmd.exe**
   EXPLANATION: msinfo32 -> Software environment -> environment variables -> ComSpec

### Task 6
1. What is the command to open Resource Monitor? (.exe not full path)
   **A: resmon.exe**
   EXPLANATION: N/A

### Task 7
1. In System Configuration, what is the full command for Internet Protocol Configuration
   **A: C:\Windows\System32\cms.exe /k %windir%\system32\ipconfig.exe**
   EXPLANATION: N/A
2. For the ipconfig command, how do you show detailed information?
   **A: **
   EXPLANATION:

### Task 8
1. What is the command to open the Registry Editor? (.exe not full path)
   **A: regedt32.exe**
   EXPLANATION: N/A
