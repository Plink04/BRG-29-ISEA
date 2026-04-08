# BRG-29-ISEA
---

__Student__: Arshvin Selva Raj <br>
__Kaplan ID__: CT0393277 <br>
__Module__: BRG-27 Introduction to Server Environments and Architectures <br>
__Host OS__: Windows 11 Home <br>
__Linux Environment__: Ubuntu 24.04.4 LTS <br>

---

# Class 1a - Intro to Linux & Installation of Ubuntu and Virtualbox
1. To begin the preparation, Ubuntu 24.04.4 LTS was downloaded
2. Virtualbox was next downloaded from its main site and a VM (Virtual Machine) was set up with the following configurations

![Lab Screenshots/Lab 1/VM Config.png](https://github.com/Plink04/BRG-29-ISEA/blob/3eb58736636205fddba734f4ea10a6542e14e166/Lab%20Screenshots/Lab%201/VM%20Config.png)

3. After setting up the VM, the Linux Home page looked like this

![Linux Home](https://github.com/Plink04/BRG-29-ISEA/blob/13de6d4f173f52c7fbc208060d27fed32a39c74c/Lab%20Screenshots/Lab%201/Linux%20Home.png)

---
# Class 1b - Linux Familiarization
1. Some tests were done to familiarize myself with the Linux GUI (Graphical User Interface)
- Testing of Firefox
![Firefox](https://github.com/Plink04/BRG-29-ISEA/blob/7c47c7fac530e26ef4a9d9475b18c0a0d83cdfde/Lab%20Screenshots/Lab%201/Firefox%20working.png)

- Installation of LibreOffice
![LibreOffice](https://github.com/Plink04/BRG-29-ISEA/blob/7c47c7fac530e26ef4a9d9475b18c0a0d83cdfde/Lab%20Screenshots/Lab%201/Lab%20Libreoffice.png)

2. Some tests were done to familiarize with the CLI (Command Line Interface)
- Using `ps-e` and `top` to see the currently running processes in the system

![Command ps-e](https://github.com/Plink04/BRG-29-ISEA/blob/7d9f51a7d30f210e7823f9ce9d281b196229877c/Lab%20Screenshots/Lab%201/Lab%20ps-e.png)

- Used `ls` , `ls-a` and `ls-la` to see files listed in a directory
- observed that certain files are not viewable in `la` and permissions of files can be seen in `ls-la`

![Command ls](https://github.com/Plink04/BRG-29-ISEA/blob/063a32f198c328b3c65ea44f54601c953e12fdd1/Lab%20Screenshots/Lab%201/Lab%20ls-la.png)

- Tested file creation with `touch`, viewing with `cat` and `less`, and editing with `gedit` and `nano`
- Observations:
- `cat` displays the file while in the CLI while `less` opens the file in a separate screen still in the CLI
![Cat](https://github.com/Plink04/BRG-29-ISEA/blob/73fc7a1fe216f793263c33e9b4c5546a19cb0c6b/Lab%20Screenshots/Lab%201/Lab%20cat.png)
![Less](https://github.com/Plink04/BRG-29-ISEA/blob/73fc7a1fe216f793263c33e9b4c5546a19cb0c6b/Lab%20Screenshots/Lab%201/Lab%20less.png)

- `gedit` opens up the file in a separate GUI for editing while `nano` has an editor while in the CLI terminal
![Gedit](https://github.com/Plink04/BRG-29-ISEA/blob/586c6db0d7ddbf055176c8382e2ab0a46f942110/Lab%20Screenshots/Lab%201/Lab%20gedit.png)
![Nano](https://github.com/Plink04/BRG-29-ISEA/blob/709b66d668d622c1f1f4bbcafd364ce327b0a69b/Lab%20Screenshots/Lab%201/Lab%20nano.png)

- Tested `whoami` and `sudo` to familiarize the different statuses of users and administrators/root
![sudo](https://github.com/Plink04/BRG-29-ISEA/blob/65308e8ae3ad4ce27401210d2f6845697b742b6e/Lab%20Screenshots/Lab%201/Lab%20superuser.png)

3. Practicing with Linux Services
   Some tests were carried out with nginx
   - Installation on CLI
   ![nginx Installed](https://github.com/Plink04/BRG-29-ISEA/blob/769d782e9cacb927ea9dedec465763e276ff6153/Lab%20Screenshots/Lab%20nginx.png)

   - NGINX websites
   ![NGINX Original](https://github.com/Plink04/BRG-29-ISEA/blob/769d782e9cacb927ea9dedec465763e276ff6153/Lab%20Screenshots/Lab%20nginx%20web.png)
   ![NGINX Ethernet](https://github.com/Plink04/BRG-29-ISEA/blob/769d782e9cacb927ea9dedec465763e276ff6153/Lab%20Screenshots/Lab%20nginx%20web%20edit%20gedit.png)
   
   - Editing using gedit
   ![gedit nginx](https://github.com/Plink04/BRG-29-ISEA/blob/769d782e9cacb927ea9dedec465763e276ff6153/Lab%20Screenshots/Lab%20nginx%20gedit.png)
   
   - Updated website 
   ![nginx edited](https://github.com/Plink04/BRG-29-ISEA/blob/769d782e9cacb927ea9dedec465763e276ff6153/Lab%20Screenshots/Lab%20nginx%20web%20edit%20gedit.png)

   Observations:
   - there is a 'not secure' notification when accessing the nginx website on different IP addresses that are not the 127.0.0.1 IP (local host)
   - sudo was needed for permission to modify the nginx web page
   - The nano and gedit modify pages for nginx were different (nano was edited on the CLI while gedit was edited in a separate GUI)

4.  Compressing and Decompressing files
   - 3 books were downloaded using the `wget` command
   ![Books downloaded](https://github.com/Plink04/BRG-29-ISEA/blob/2e9974546b7c1b045b2df3a4ae7f659af61e4e4f/Lab%20Screenshots/Lab%20Gutenberg%20install.png)
   
   - A directory was made using `mkdir` and the books were moved there using `mv`
   ![Books moved](https://github.com/Plink04/BRG-29-ISEA/blob/2e9974546b7c1b045b2df3a4ae7f659af61e4e4f/Lab%20Screenshots/Lab%20Gutenberg%20books%20moved.png)

   - The books were then compressed with `tar` and `bzip2`
   ![Books compressed](https://github.com/Plink04/BRG-29-ISEA/blob/2e9974546b7c1b045b2df3a4ae7f659af61e4e4f/Lab%20Screenshots/Lab%20Gutenberg%20books%20zip.tar.png)
   
   - Command `ls-la` to compare file sizes 
   ![books ls](https://github.com/Plink04/BRG-29-ISEA/blob/2e9974546b7c1b045b2df3a4ae7f659af61e4e4f/Lab%20Screenshots/Lab%20Gutenberg%20books%20ls.png)

   - The books file was then decompressed
   ![Books decompressed](https://github.com/Plink04/BRG-29-ISEA/blob/2e9974546b7c1b045b2df3a4ae7f659af61e4e4f/Lab%20Screenshots/Lab%20Gutenberg%20books%20decompress.png)
   
Reflection:
- There were a lot of different commands, concepts and terminologies to understand, as this is my first time learning about linux and IT. Commands can be searched up with `man` but will take adequate practice to fully understand and master the usages. 
- Not many issues were encountered as installation processes and command practices were very direct

---
# Class 2a
1. Total Cost of Ownership
Below is the excel sheets of the calculations made between 2 types of printers, an inkjet versus a laser printer.
![TCO](https://github.com/Plink04/BRG-29-ISEA/blob/5413e1e4355ad4b68a19af429c5e98bcd5c1ae61/Lab%20Screenshots/TCO%20PrinterS.png)

Reflection:
- There is a significant difference in cost between the inkjet printer and the laser printer, with the inkjet one being way more cost efficient for over a period of 5 years.
- Home users who wont print as much as compared to offices (eg. 5 pages a week) are more likely to choose an inkjet printer to own, or maybe even consider just using printing services near their homes.
- Some external non-financial factors to consider:
  - Preference to certain brands
  - Convenience of usage for the printer of use
  - Availability and usefulness of customer support services for the printer
  - Speed of printing
- For larger workgroup printers, the main cost factors to consider would be ink bottle/cartridge/drum costs, maintenance or printer replacement costs and Paper costs.
- The laser printer will most likely never break even to the inkjet printer due to the vast difference in cost for their ink cartridges/drums. 
---
# Class 2b
1. Cloud Computing
 - For this exercise, a Virtual Machine was set up using AzureVM
 - Settings were adjusted accordingly to fit the criteria of the exercise
 - After setting up, the AzureVM was connected to my desktop using the generated pem.key
![Azure connected](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/Azure%20host.png)

 - NGINX was installed and configured to the public IP of the VM
![Azure Nginx](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/NGINX%20Azure.png)

- Further practice was done by editing using nano
![NGINX Practice](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/Azure%20edited.png)

- Another exercise was done by linking a downloaded file to the IP
![NGINX Practice 2](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/Azure%20edited2.png)

- Some issues faced during the process of setting up of Azure:
  - Difficulty with navigating the GUI of Azure due to how many settings there were
  - Issues with connecting the powershell to AzureVM with the key due to incorrect/invalid commands
  - connection issues during the process of configuring NGINX

Reflection: 
- Learnt more about the inner workings of Cloud servers
- Certain ports such as `80`, `443`, need to be enabled for connection to web browsers

2. Introduction to Bash coding
- Bash navigating system and managing files
- after familiarizing with some of the CLI commands from the previous class, the following steps were taken to carry out some activities in Bash.
  - Using `mkdir` to create a new directory, `touch` to create a new file and `echo` to edit the contents inside the file.
![Bash Note activity 1](https://github.com/Plink04/BRG-29-ISEA/blob/d0cb3185cbf5b7f75fe5bb30039ded299813bf47/Lab%20Screenshots/Lab%203/Lab%20Bash%20note.png)

 - More practices with different commands such as `cat` to display the file contents in CLI and `cp`, `mv` and `rm` to copy, rename and remove the file respectively.
![Bash Note activity 2](https://github.com/Plink04/BRG-29-ISEA/blob/d0cb3185cbf5b7f75fe5bb30039ded299813bf47/Lab%20Screenshots/Lab%203/Lab%20Bash%20note%202.png)

Reflection: 
- The command `mkdir` is used for making directories
- The command `cat` can be used to display the contents of a file without having to access a GUI, similar (but different) to the command `nano`
- The `cp` command is used to create a copy of a file but with a different name, while the `mv` command is used for renaming files

- After the notes practice, some exercises were done for creating and executing Bash scripts
  - Exercise to create a Bash script to generate a line of text
  ![Bash Script Hello World](https://github.com/Plink04/BRG-29-ISEA/blob/d0cb3185cbf5b7f75fe5bb30039ded299813bf47/Lab%20Screenshots/Lab%203/Lab%20Bash%20Script%20amended.png)

  - Exercise to create a loop and conditional script for inputting and detecting a value from 1-10 
  ![Bash Script Loop](https://github.com/Plink04/BRG-29-ISEA/blob/d0cb3185cbf5b7f75fe5bb30039ded299813bf47/Lab%20Screenshots/Lab%203/Lab%20Bash%20System%20Info%20Script.png)

  - Exercise to create a system resource monitor
  ![Bash System Resource Monitor](https://github.com/Plink04/BRG-29-ISEA/blob/d0cb3185cbf5b7f75fe5bb30039ded299813bf47/Lab%20Screenshots/Lab%203/Lab%20Bash%20Resource%20Monitor.png)

Reflection: 
- Learnt that the `chmod` command is used to give permissions to allow a script to be executed as a programme
- The shebang (#!/bin/bash) is to be added at the start of the script so that it can be identified and ran using Bash Shell
- The main command I used for modifying personalized messages in scripts was using the `nano` command, and modifying the message indicated to be displayed with the `echo` command
- The `for loop` is used when repeating a set of commands within a certain range of values/inputs
- In the loop script exercise, the script was done such that if a value that was outside the set perimeter was keyed in, the condition to trigger the `else` command would be active run its script.
- The following command, `! [[ "$number" =~ ^[0-9]+$ ]]` was used to handle invalid inputs for the if loop
- Was unsure at first, but found out that the `free -h` command is used to display information about the systems memory usage in a human readable format, hence the `-h`
- To modify the script to monitor system usage, certain commands such as `htop` or `free -h`

  ---
# Class 3a

1. DNS
   - Setting up a Domain using `DuckDNS`
   - A domain was created with the URL `azurequack.duckdns.org`
   ![DuckDNS](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/Domain%20.png)

   - The domain was then updated with the IP address of the Public IP in AzureVM
   ![Domain IP](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/Domain%20updated%20IP.png)

   - Verified that the domain was working using commands such as `nslookup` and `dig`
   ![NSLookup](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/DNS%20NSlookup.png)


![Dig](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/DNS%20Dig.png)

2. Digital Certificates

- Certbot and Apache2 were installed through the CLI on Azure
- Had some issues at first as NGINX had to be disabled first to connect the domain to Apache2

![Cert Apache2](https://github.com/Plink04/BRG-29-ISEA/blob/0ffc8c6ec27e4898b52204b3e327050bf469060a/Lab%20Screenshots/Lab%202/DNS%20Apache2.png)

---
# Class 3b
1. Scripting Linux Server Functions




---
# Class 4 - Additional Server services
1. Chose Docker as the additional server service to download

- System preparations were made to Ubuntu using the following commands: <br>
`sudo apt update` <br>
`sudo apt upgrade -y` <br>
`sudo apt install -y curl wget gnupg lsb-release ca-certificates` <br>

- Docker was then installed through the CLI and Docker Desktop
![Docker installation 1](https://github.com/Plink04/BRG-29-ISEA/blob/26b117a0a86f126abbab4eb672643c0d9e1f20f5/Lab%20Screenshots/Lab%20Installing%20Docker%201.png)
![Docker installation 2](https://github.com/Plink04/BRG-29-ISEA/blob/26b117a0a86f126abbab4eb672643c0d9e1f20f5/Lab%20Screenshots/Lab%20Installing%20Docker%202.png)

- Verification to show that Docker was successfully installed
![Docker Verify](https://github.com/Plink04/BRG-29-ISEA/blob/26b117a0a86f126abbab4eb672643c0d9e1f20f5/Lab%20Screenshots/Lab%20Installing%20Docker%20hello%20world.png) 


