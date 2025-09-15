# **EXPERIMENT 2**
# **Linux File systems Permissions & Essential Commands**
--------------------------------------------------------------------------
## 📌 Aim
To understand the structure of the Linux file system, manage file permissions and ownership, and practice essential Linux commands.

---------------------------------------------------------------------------
## 🛠 Tools & Software Used 
- **Operating System:** Ubuntu running on Oracle VirtualBox  
- **Terminal Emulator:** GNOME Terminal 
- **Shell:** Bash (*Bourne-Again Shell*)

---------------------------------------------------------------------------
## 📂 <u>Linux File Systems</u>
- The Linux file system is a structured and hierarchical way of storing and organizing files and directories.
- Linux treats everything as part of a single directory tree starting from the root directory `/`
- To view all files and directories in the root `/` directory along with their details such as *permissions*, *ownership*, etc.
we can use comand
```
ls -l /
```
 ### Output:
  ![output](images/201.png) <br><br>

---------------------------------------------------------------------------
## 🔑 <u>File Permissions and Ownership</u>
- Every file and directory in Linux has three types of permissions:
  - `r` *read*
  - `w` *write*
  - `x` *execute*

- Categories of Users:
  - Owner
  - Group 
  - Ohters

- Using `ls -l` command to see the permission and ownership for a file `file1.txt`

 ### Output:
 ![output](images/202.png) <br><br>

---------------------------------------------------------------------------

## ⚙️ <u>Modifying Permissions</u>
  ### Using `chmod` command
- To change the permission and making `myfile.txt` executable for the user we can use the command
```
chmod u+x myfile.txt
```
 ### Output:
 ![Output](images/203.png)<br><br>
- We can also change permission using numeric mode 
```
chmod 744 myfile2.txt
chmod 754 myfile2.txt
```
 ### Output:
 ![Output](images/204.png)<br><br>

---------------------------------------------------------------------------

## 📍 <u>Basic Navigation Commands</u>

### 1. `ls` - List Directory content
- `ls` - *List files in current directory*
- `ls - l` - *List with detailed information*
- `ls - a` - *List all files using hidden ones*
- `ls - la` - *Combined option for viewing detailed view with hidden files*

 ### Output:
- `ls`:
![Output](images/205.png) <br><br>
- `ls -l`:
![Output](images/206.png) <br><br>
- `ls -a`:
![Output](images/207.png) <br><br>
- `ls -la`:
![Output](images/208.png) <br><br>

---------------------------------------------------------------------------
### 2. `pwd` - Print working Directory
- Shows your current location in the file.
 ### Output:
 ![Output](images/209.png) <br><br>

---------------------------------------------------------------------------
### `cd` - Change Directory
- `cd`- *Go to home directory*
- `cd /home/vivekchauhan12/Downloads/lab2`- *Go to a specific directory*
- `cd ..` - *Go up one level*
- `cd -` - *Go to previous directory*
- `cd /` - *Go to root directory*
 #### Output:
  ![Output](images/210.png) <br><br>

---------------------------------------------------------------------------
### 3. `mkdir` - Make directory 
 #### Syntax
  ```
  mkdir [options] directory_name
  ```
- **Creating a single directory**
   `mkdir directory_name`<br><br>

- **Creating multiple directories at once**
   `mkdir directory_1 directory_2 directory_3`<br><br>

- **Creating nested directories**
   `mkdir -p parent_directory/child_directory`<br><br>

- **Creating directory with special permissions**
   `mkdir -m mode directory_name`<br><br>

 #### Output:
 ![Output](images/211.png) <br><br>

---------------------------------------------------------------------------
### 4. `rmdir` - Remove Empty Directory
 #### Syntax
 ```
 rmdir [options] directory_name
 ```
- **Remove an empty directory**
   `rmdir directory_name`<br><br>

- **Remove multiple empty directories**
   `rmdir directory_1 directory_2 directory_3`<br><br>

- **Remove nested empty directories**
   `rmdir -p parent_directory/child_directory`<br><br>

 #### Output:
  ![output](images/212.png) <br><br>

---------------------------------------------------------------------------
## 📝 <u>File Operations</u><br><br>

 ### 1. `touch` - Creates files
  -  The `touch` command is used to create empty files or to update timestamps of existing flies. 
  #### Syntax
   ```
    touch [options] file_name

   ```
   - **Creating a single file**
      `touch file_name`<br><br>

   - **Creating multiple files at once**
      `touch file1_name file2_name file3_name`<br><br>

   #### Output:
   ![output](images/213.png)<br><br>

---------------------------------------------------------------------------
 ### 2. `cp` - Copying files and directories
  
  - The `cp` command is used to copy files from one location to another.  
  #### Syntax 
  ```
  cp [options] source destination
  ```
  - **Copy a single file** - Copies the content of source file to destination file.
    `cp source_file destination_file`<br><br>
  
  - **Copy multiple files to a directory** - Copies all the files to the given destination directory at once.
    `cp source_files destination_directory_path`<br><br>

  - **Copy a directory recusively** - Copy all the files and sub directories of source directory to the destination directory.
    `cp -r [source] [destination]`<br><br>
  
  - **Copy and show details** - Display each file being copied.
    `cp -v [source] [destination]`<br><br>

  - **Copy with confirmation** - prompts for confirmation before overwriting a file.
    ` cp -i [source] [destination]`<br><br>

  #### Output:
  ![Output](images/214.png)<br><br>

---------------------------------------------------------------------------
 ### 3. `mv` - Move and rename
  - `mv` command is uesed to move files and directories from one place to another.
  
  #### Syntax 
  ```
   mv [options] source dstination
  ```
  - **Move file to different directory**
    `mv source_file destination_directory`<br><br>
  
  - **Move multiple files**
    ` mv source_files destination_directory`<br><br>

  - **Rename a file**
    ` mv old_name new_name`<br><br>
  
  - **Rename a directory**
    ` mv old_name new_name`<br><br>

  #### Output:
  ![output](images/215.png) <br><br>

---------------------------------------------------------------------------
 ### 4. `rm` - Remove files and directories
  - `rm` command is used to remove files permanently.
 
  #### Syntax
  ```
  rm [options] file_name
  ```
  - **Remove a file**
    `rm file_name` <br><br>

  - **Remove multiple files**
    ` rm file_names` <br><br>
 
  - **Remove directory and its content**
    ` rm -r directory_name` <br><br>

  - **Forced removal without confirmation**
    ` rm -f file_name` <br><br>

  - **Confirmable removal**
   ` rm -i file_name` <br><br>

  #### Output:
  ![output](images/216.png) <br><br>

---------------------------------------------------------------------------
## 👀 <u>File viewing and Editing</u><br><br>

 ### 1. `cat` - Used for viewing, creating and merging files
  - The `cat` command is use to display the content of files, create new fiels or combine multiple files.
  
  #### Syntax
  ```
  cat [options] file_name
  ```

  - **To display the content of files**
    `cat file_name` <br><br>
  
  - **To display multiple files together**
    ` cat file_names` <br><br>
  
  - **To create a new file**
    ` cat > file_name` <br><br>

  - **Merging files into a new file**
    ` cat file1 file2 > file_name` <br><br>
  
  - **To display all output lines with numbers**
    ` cat -n file_name` <br><br>

   - **To display all non empty output lines with numbers**
    ` cat -b file_name` <br><br>

  #### Output:
  ![output](images/217.png)<br><br>
  ![output](images/218.png)<br><br>

---------------------------------------------------------------------------
 ### 2. `head` - Viewing the beginning of files
  - The `head` command is used to view first few lines of a file.

  #### Syntax 
  ```
  head [options] file_name
  ```

  - **To display the first 10 lines of a file (*default*)**
    ` head file_name`<br><br>
  
  - **To display the first 5 lines**
    `head -n 5 file_name`<br><br>
  
  - **To display first 20 bytes of a file**
    ` head -c 20 file_name`<br><br>

  #### Output:
  ![Output](images/219.png)<br><br>

---------------------------------------------------------------------------
 ### 3. `tail` - Viewing the end of files
  - The `tail` command is used to view last few lines of a file.

  #### Syntax
  ```
  tail [options] file_name
  ```
  - **To display the last 10 lines of a file (*default*)**
    ` tail file_name`<br><br>
  
  - **To display the last 5 lines of a file (*default*)**
    ` tail -n 5 file_name`<br><br>

  - **To display last 20 bytes of a file**
    ` tail -c 20 file_name`<br><br>
  
  - **To monitor a file in real time**
    ` tail -f file_name` <br><br>

  #### Output:
  ![output](images/220.png)<br><br>
  ![output](images/221.png)<br><br>

---------------------------------------------------------------------------
## ✍️ <u>Text editors</u><br><br>
 ### 1. Nano
  - NANO is a text editor that works directly from the terminal, ysefult o create and edit files.
  
  #### Output:
   ![output](images/222.png)<br><br>
   ![output](images/223.png)<br><br>

---------------------------------------------------------------------------
 ### 2. Vim
  - VIM is an advanced text editor with features like syntax higlighting, efficient navigation and powerful editing commands.

  #### OUTPUT:
   ![output](images/224.png)<br><br>
   ![output](images/225.png)<br><br>

---------------------------------------------------------------------------

## 👤 <u>User Management</u><br><br>
 ### 1. `whoami` - Display the current username 

 ### 2. `who` - Display all users currently logged into the system

 ### 3. `passwd` - To change user password

 ### 4. `sudo ` - To run commands with administrative priviliges
  - For tasks like updating and installing packages, ediitng the system files `sudo` command is used.
  - `sudo` grants root priviliges to the user to run commands.
  #### Syntax
   ```
    sudo command
   ```
  
 ### OUTPUT:
  ![output](images/226.png)
  ![output](images/227.png)<br><br>

---------------------------------------------------------------------------
  
 ## 🖥️ <u>System Information</u><br><br>
  ### 1.`uname` - To display detais about linux system

   #### Syntax
   ```
    uname [options]
   ```
   - **To display basic system info**
     `uname`<br><br>
    
   - **To display all system info**
     `uname -a`<br><br>

   - **To display kernel version**
     `uname -r`<br><br>

   - **To display machine hardware info**
     `uname -m`<br><br>

   - **To display OS info**
     `uname -o`<br><br>

   #### OUTPUT:
   ![output](images/228.png)<br><br>

---------------------------------------------------------------------------
  ### 2.`df` - To display the information about disk space usage
   
   #### Syntax
   ```
   df [options] [file_systems]
   ```
   - **To display basic disk usage**
    `df`<br><br>

   - **To display disk usage in human readable format**
    `df -h`<br><br>

   - **To display file system type**
    `df -T`<br><br>
  
   #### OUTPUT:
   ![output](images/229.png)<br><br>

---------------------------------------------------------------------------

  ### 3.`top` - shows real time information 
   - `top` shows real time info about processes, CPU usage, memory usage and other system resources

  ### OUTPUT:
   ![output](images/230.png)<br><br>

---------------------------------------------------------------------------
  ### 4. `history` - shows a list of commands that have been executed in the terminal

   #### Syntax 
   ```
   history
   ```
   - **To display command history**
     `history`<br><br>

   - **To display last n commands**
     `history n`<br><br>

   - **To search history**
     `history | grep "search_term"` <br><br>
   
   - **Execute previous command**
     `!!<br><br>

   #### OUTPUT:
   ![output](images/231.png)<br><br>

---------------------------------------------------------------------------
## 🧩 <u>EXERCISES</u>
 ### Exercise 1 - File system navigation<br><br>
  ![output](images/232.png)<br><br>

---------------------------------------------------------------------------
 ### Exercise 2 - File operations and permissions<br><br>
  ![output](images/233.png)<br><br>

---------------------------------------------------------------------------
 ### Exercise 3 - Text Editing and viewing<br><br>
  ![output](images/234.png)<br><br>

---------------------------------------------------------------------------
 ### Exercise 4 - System exploration<br><br>
  ![output](images/235.png)<br><br>

---------------------------------------------------------------------------
 ### Exercise 5 - Cleanup <br><br>
 ![output](images/236.png)<br><br>

---------------------------------------------------------------------------
## 📋 OBERVATIONS
 
 - The Linux file system structure was explored using commands.

 - File permissions and ownership were checked and modified.

 - Directories were navigated, and file operations were performed.

 - File contents were viewed and edited with text editors.

 - User management tasks were carried out using appropriate commands.

 - System information and resource usage were monitored during the experiment.

-----------------------------------------------------------------------------

## 🧠 CONCLUSION
 The experiment provided practical experience in using various Linux commands related to file systems, permissions, navigation, file operations, editing, user management, and system monitoring.

------------------------------------------------------------------------------
