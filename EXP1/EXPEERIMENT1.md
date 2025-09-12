# **EXPERIMENT 1** 
## *Installation of VirtualBox and Setting up linux OS*
---
## 📌 Aim  
To install **Oracle VirtualBox** on a Windows system and set up a Linux operating system (Ubuntu/Fedora/etc.) to practice Linux commands and explore its environment in a virtual machine.

---
## 🛠 Tools & Software Used  
- **Host OS:** Windows 11
- **Virtualization Software:** Oracle VirtualBox *v7.2.0*
- **Guest OS:** Ubuntu 24.04.03

---
## 📋 Procedure
### **Step 1-** Downloading the Oracle Virtual Box
- Open [https://www.virtualbox.org/](https://www.virtualbox.org/) 
- Download the latest version for Windows hosts
![Downloading VirtualBox](images/111.png)
### **Step 2-**  Download an installation .iso for a Linux distribution like Ubuntu
-  An .iso file is a disk image of the Linux distribution you want to install. It contains all the necessary files for the operating system.
 
![downloading .iso file](images/114.png)
### **Step 3-** Installing the VirtualBox
- Run the downloaded installer.<br><br>


- Follow the installation steps and accept default options.
![Installing VirtualBox](images/112.png)  <br><br>


- Launch Oracle VirtualBox after installation.
![Launching VirtualBox](images/113.png)<br><br>

### **Step 4-** Creating a new Virtual machine -  Ubuntu 
- Create a new virtual machine by clicking on the "New" or "Create" button.
![Creating a new VM](images\115.png) <br><br>


- Follow the on-screen instructions to set up the virtual machine. This includes specifying the name, location, and specifications for the virtual machine, such as the amount of RAM and storage allocated.  
![RAM & Storage allocation](images/116.png) <br><br>


- A summary will be shown about the VM to be created
![Summary of vM](images\117.png)<br><br>


- Adding `ubuntu-24.04.3-desktop-amd64.iso` file in **Stoage** under the **Controller:IDE** by clicking on the empty optical drive.
![Adding .iso file](images/118.png)<br><br>


- Completing the virtual machine setup by following the remaining on-screen instructions involving configuring network settings, and specifying storage options,etc.
![Configuring](images/119.png)<br><br>


- Installing and setting up the `Ubuntu 24.04` by following th einstalltion prompts and providing the required information such as username, password.
![Setting up Ubuntu](images/120.png)<br><br>


- After the installation is complete we will have a fully functional **Linux Virtual Machine** running with **VirtualBox**.
![Linux VM](images/121.png)

---
## ✅ Observations

- Oracle VirtualBox was installed successfully without any issues.
- The Linux OS booted and installed properly inside the virtual machine.
- Terminal commands were executed successfully.

---
## 🧠 Conclusion

The experiment helped me install and configure Oracle VirtualBox and set up a Linux operating system in a virtual environment.


