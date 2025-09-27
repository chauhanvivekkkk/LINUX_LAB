# <h1 style="background-color: orange;"> EXPERIMENT 8 - Shell Programming</h1>

---------------------------------------------------------------------------
## 📌 Aim
   **To understand and demonstrate the concepts of process control and signals, process monitoring and resource usage, process communication and synchronization, background processes and job control, and system monitoring and logging in Linux**

---------------------------------------------------------------------------
## 🛠 Tools & Software Used 
- **Operating System:** Ubuntu running on Oracle VirtualBox  
- **Terminal Emulator:** GNOME Terminal 
- **Shell:** Bash (*Bourne-Again Shell*)

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">Process Control & signals</h1>
 #### - `   kill   ` - used to terminate or send signals to processes
 
 #### Syntax:
 ````

   kill [options] <PID>

 ````
  #### Signals (used as options):
   1. `  2  ` - **SIGINT** (*interrupt*)
   2. `  15  ` - **SIGTERM** (*termiante gracefully*)
   3. `  9  ` - **SIGKILL** (*force kill*)
   4. `  19  ` - **SIGSTOP** (*Stops a process*)
   5. `  18  ` - **SIGCONT** (*resumes the stopped process*)

 #### OUTPUT:

 ![output1](images/801.png)

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">Process Monitoring and Resource Usage</h1>

 #### Commands:
 1. `   top    ` - **live view of processes, CPU, memory**
 2. `   htop    ` - **user friendly version of *top***
 3. `   ps aux    ` - **snapshot of all processes**
 4. `   free -h  ` - **show memory usage**
 5. `   uptime    ` - **system load avrages**

 #### OUTPUT:
 ![output2](images/802.png)

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">Process Communication</h1>
 
- **Pipes `  |  ` - to pass output of one command to another**

 #### OUTPUT:
 ![output3](images/803.png)

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">Process Synchronization</h1>
  **To prevent conflicts, processes can be synchronized**
  - `   wait  ` - **used to pause the execution of a script until all the background processes complete.**

  - ` wait <PID> ` - **waits for a particular job to finish**

#### OUTPUT:
![output4](images/804.png)

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">Background Process and Job control</h1>

 - `   &   ` - **used to run a process in background**
 - `  jobs  ` - **shows background jobs**
 - `   fg %1   ` - **brings job 1 to foreground**
 - `   bg %1   ` - **resume job 1 in background**

 #### OUTPUT:
 ![output5](images/805.png)

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">System Monitoring and logging</h1>

 - `  dmesg | less  ` - **kernel/ system messages**
 - `  journalctl  ` - **systemlogs**
 - `  last  ` - **logged-in users**
 - `  who  `  or  `  w  ` - **user currently logged-in**

#### OUTPUT:
![output6](images/806.png)

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">🧩LAB Exericeses</h1>
### <h1 style="background-color: lightgreen;">TASK 1: Check File Permissions</h1>
   #### Script:
   ![script1](images/807.png)<br><br>
  
   #### Output:
   ![output7](images/808.png)<br><br>

### <h1 style="background-color: lightgreen;">TASK 2: String Operations</h1>
   #### Script:
   ![script2](images/809.png)<br><br>
  
   #### Output:
   ![output8](images/810.png)<br><br>

### <h1 style="background-color: lightgreen;">TASK 3: Search for a Pattern in a file</h1>
   #### Script:
   ![script3](images/811.png)<br><br>
  
   #### Output:
   ![output9](images/812.png)<br><br>

### <h1 style="background-color: lightgreen;">TASK 4: Display System Information</h1>
   #### Script:
   ![script4](images/813.png)<br><br>
  
   #### Output:
   ![output10](images/814.png)<br><br>

---------------------------------------------------------------------------
## <h1 style="background-color: pink;">📋 OBSERVATIONS</h1>

 - `kill`, `wait` and job control commands (`&`, `jobs`, `fg`, `bg`) worked as expected.

 - `top`, `htop`, `ps aux`, and `free -h` provided real-time process and resource information.

 - Pipes (`|`) enabled inter-process communication.

 - System monitoring commands (`dmesg`, `journalctl`, `last`, `who`) displayed logs and user activity correctly.

 - Lab exercises executed successfully with expected outputs.
 
---------------------------------------------------------------------------
## <h1 style="background-color: pink;">🧠 CONCLUSION</h1> 

- The experiment demonstrated process control, monitoring, communication, and synchronization in Linux.

- Background job management and system monitoring help efficiently manage processes.

- Shell scripting with process commands enables effective automation and resource tracking.

---------------------------------------------------------------------------
---------------------------------------------------------------------------