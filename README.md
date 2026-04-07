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
- TCO
- Introduction to Bash coding
- Bash navigating system and managing files
  
# Class 3
- DNS
- Digital Certificates

# Class 4
