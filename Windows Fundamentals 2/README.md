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
#### System Tools

#### Storage

#### Services and Applications

## Computer Management

## System Information

## Resource Monitor

## Command Prompt

## Registry Editor

## Answers to Questions
### Task 2
1. What is the name of the service that lists Systems Internals as the manufacturerer?
   **A: PsShutdown**
   EXPLANATION: Found in the Services tab of **System Configuration**
2. Whom is the Windows license registered to?
   **A: Windows User**
   EXPLANATION: search bar-> msconfig -> tools -> About Windows -> Launch -> Windows User (at the bottom)
3. What is the command for Windows Troubleshooting
   **A:**
   EXPLANATION:
4. What command will open the control Panel? (the .exe not the full path)
   **A:**
   EXPLANATION:
