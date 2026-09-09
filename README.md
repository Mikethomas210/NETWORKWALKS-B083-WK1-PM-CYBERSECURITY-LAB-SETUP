# NETWORKWALKS-B083-WK1-PM-CYBERSECURITY-LAB-SETUP
A hands-on cybersecurity lab documenting Kali Linux deployment, VirtualBox configuration, network setup, connectivity testing, and VM snapshots.

 OBJECTIVE
Set up a Kali Linux VM with internet access using NAT network and document the process for learning and reproducibility.

TOOLS USED
7-Zip: For extracting Kali ISO file
Oracle VirtualBox
Kali Linux ISO**: Latest version from kali.org
Host OS: Windows 11

 Step-by-Step Guide

 Step 1: Install 7-Zip
1. Download 7-Zip from the official website.
2. Run the installer and complete setup.
3. Use 7-Zip to extract the downloaded Kali Linux ISO

  Step 2: Install Oracle VirtualBox
1. Download Oracle VirtualBox from virtualbox.org
2. Run the installer > Next > Install

    Step 3: Download Kali Linux
1. Go to kali.org > Downloads
2. Download `Kali Linux Installer ISO 64-bit`
3. Extract with 7-Zip if needed.

    Step 4: Create Kali VM in VirtualBox
1. Open VirtualBox > Click `New`
2. Name: `Kali-Linux`
3. Type: `Linux` | Version: `Debian (64-bit)`
4. RAM: `4096 MB` minimum
5. Create Virtual Hard Disk: `VDI`, `Dynamically allocated`, `20GB`
6. Settings > Storage > Add Kali ISO to Optical Drive

7. Step 5: Configure Network to NAT NETWORK
1. Settings > Network > Adapter 1
2. Attached to: `NAT`NETWORK
3. Click `OK`
   > NAT NETWORK allows the VM to access internet through host without exposing it to local network.

    Step 6: Install Kali Linux
1. Start VM > Select `Graphical Install`
2. Follow prompts: Language, Keyboard, Hostname, User/Password
3. Partition disk > Finish installation > Reboot

4. Step 7: Test Network Connection
1. Log in to Kali
2. Open `Firefox ESR` from Applications Menu
3. Navigate to `google.com` to confirm internet access via NAT

4.  Step 8: Take a Snapshot
1. Shut down Kali VM
2. In VirtualBox: Right-click VM > `Snapshots` > `Take Snapshot`
3. Name: `Fresh-Install-Network-Working`
   > This saves the current state so you can revert if something breaks.

    Verification
 Kali boots successfully
 Internet works on NAT - tested with google.com
Snapshot created

 Screenshots
Add screenshots here of:
1. VirtualBox settings - Network NAT
2. Firefox on Kali showing google.com
3. Snapshot in VirtualBox

Author: Thomas Michael Anayochukwu
Date: 9th September 2026
