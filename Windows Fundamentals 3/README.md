# TRY HACK ME - Windows Fundamentals 3
## Windows Updates
- access Windows Update from the CMD by running the command **control /name Microsoft.WindowsUpdate**

## Windows Security
- used to manage the tools that protect your device and data
- there are three different colour status icons:
  1. Green means your device is sufficiently protected, and there aren't any recommended actions
  2. Yellow means that there is a safety recommendation for you to review
  3. Red is a warning that something needs your immediate attention

## Virus & Threat Protection
### Current threats
- scan options:
  1. quick scan: checks folders in your system where threats are commonly found
  2. full scan: checks all files and running programs on your hard disk. This scan could take longer than one hour
  3. Custom scan: choose which files and locations you want to check
 
- Threat history:
  1. last scan: widnows defender antivirus automatically scans your device for viruses and other threats to help keep it safe
  2. quarantined threats: quarantined threats have been isolated and prevented from running on your device
  3. allowed threats: Allowed threats are items identified as threats, which you allowed to run on your device
 
  ### Virus & threat protection settings
  #### manage settings
  - real-time protection: locates and stops malware from isntalling or running on your device
  - Cloud delivered protection: provides increased and faster protection with access to the latest protection data in the cloud
  - automatic sample submission: send sample files to microsoft to help protect you and others from potential threats
  - controlled older access: If enabled, this feature protects files, folders and memory areas on your device from unauthorized changes by malicious or unknown applications. Enable by clicking on **manage controlled folder access** under **controlled folder access**
  - Exclusions: Windows Defender Antivirus allows you exclude any files or folders from the antivirus scanning in order to reduce the nuumber of false positives
  - Notifications: Windows Defender Antivirus will send notificiations with ciritical information about the health and security of your device

## Firewall & Network Protection
- a firewall is what controls what is and isn't allowed to pass through ports
- three groups that can interact with a firewall:
  1. Domain: the domain profile applies to networks where the host system can authenticate to a domain controller
  2. Private: the private profile is a sure-assigned profile and is used to designate private or home networks
  3. Public: the default public profile is used to designate public networks such as Wi-Fi hotspots at coffee shops, airports and other locations

## App & Browser Control
- Microsoft Defender SmartScreen protects against phishing or malware websites and applications and the downloading of potentially malicious files

## Device Secuirty
### Core Isolation
- Security features available on your device that use virtualization-based security
- Memory Integrity: prevents attacks from inserting malicious code into high-security processes

### Security Processor
- your security processor, called the **trusted platform module (TPM)**, is providing additional encryption for your device
- The TPM is designed to provide hardware-based, security-related functions
- A TPM chip is a secure crypto-processor that is designed to carry out cryptographic operations. The chip incldues multiple physical security mechanisms to make it tamper-resistant, and malicious software is unable to tamper with the security functions of the TPM

## BitLocker
- BitLocker is a data protection feature, integrated with the OS to address data theft, exposure from lost/stolen/inappropriately decomissioned computers

## Volume Shadow Copy Service
- the Volume Shadow Copy Service (VSS) coordinates the required actions to created a consistent shadow copy of the data that is to be backed up
- With VSS enabled the following tasks can be performed:
  - Create a restore point
  - perform system restore
  - configure restore settings
  - delete restore points

## Answers to Questions

### Task 2 Questions
1. There were two definitions updates installed in the attached VM. On what date were these updates installed?
   **A: 5/3/2021**
   EXPLANATION: cmd -> control /name Microsoft.WindowsUpdate -> View update history -> Definition Updates

### Task 3 Questions
1. Checking the Security section on your VM, which area needs immediate attention?
   **A: virus & threat protection**
   EXPLANATION: windows update -> Windows security -> open windows security -> virus & threat protection

### Task 4 Questions
1. Specifically, what is turned off that Windows is notifying you to turn on?
   **A: real-time protection**
   EXPLANATION: N/A

### Task 5 Questions
1. If you were connected to airport Wi-Fi, what most likely will be the active firewall profile?
   **A: public network**
   EXPLANATION: N/A

### Task 7 Questions
1. What is the TPM?
   **A: Trusted Platform Module**
   EXPLANATION: N/A

### Task 8 Questions
1. We should use a removeable drive on systems without a TPM version 1.2 or later. What does this removeable drive contain?
   **A: startup key**
   EXPLANATION: N/A

### Task 9 Questions
1. What is VSS?
   **A: Volume Shadow Copy Service**
   EXPLANATION: N/A
