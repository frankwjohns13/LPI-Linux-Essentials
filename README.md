![LPI Linux Essentials](https://www.lpi.org/wp-content/webp-express/webp-images/uploads/2023/04/Essentials-Linux.jpg.webp)

# LPI Linux Essentials - Exam Notes

## Topic 1: The Linux Community and a Career in Open Source (Weight: 7)

### 1.1 Linux Evolution and Popular Operating Systems (Weight: 2)
Knowledge of Linux development and major distrobutions.

**Key Knowledge Areas:** 
- Major Linux distributions and their use cases
- Embedded systems and specialized Linux versions
- Linux in the cloud

**Important Concepts & Terms:**
- **Distributions (Distros)**:
  - **Debian-based**: Debian, Ubuntu (Long Term Support (LTS) versions are popular for servers)
  - **Red Hat-based**: Red Hat Enterprise Linux (RHEL), CentOS, Fedora
  - **SUSE-based**: OpenSUSE, SUSE Linux Enterprise
  - Others: Linux Mint (User-friendly), Raspberry Pi OS (for Pi devices)
- **Embedded Systems**: Lightweight Linux versions used in devices like routers, IoT, cars, etc. (e.g., Raspbian on Raspberry Pi, Andriod is Linux-based).
- **Linux in the Cloud**: Most cloud servers run Linux (Ubuntu, Amazon Linux, etc.). Containers (Docker) and orchestration (Kubernetes) are heavily Linux-based.
- **Kali**: Designed packed full of applications used in penetration testing (Okay, this may not be on the test, but I think everyone should know it)

**Exam Tips:**
- Know the most popular server distros: Ubuntu and RHEL/CentOS
- Understand that Android is a Linux-based operating system
  
### 1.2 Major Open Source Applications (Weight: 2)
Awareness of major applications as well as their uses and development. 

**Key Knowledge Areas:** 
- Desktop applications
- Server applications
- Development languages
- Package management tools and repositories

**Important Concepts & Terms:**
- **Desktop applications**
  - LibreOffice / OpenOffice (office suite)
  - Firefox (web browser)
  - Thunderbird (email client)
  - GIMP (image editing - like Photoshop) 
- **Server applicatons**
  - Apache HTTPD & NGINX (web servers)
  - MariaDB / MySQL (database)
  - Samba (file sharing with Windows)
  - Nextcloud / ownCloud (private cloud storage)
- **Development languages**
  - C, Java, JavaScript, Perl, shell, Python, PHP
- **Package management and repositories**
  - **Debian/Ubuntu**: apt, apt-get, dpkg
  - **Red Hat/CentOS/Fedora**: yum, dnf, rpm

**Exam Tips:**
- Know the difference between apt (Debian) and yum/dnf (Red Hat).
- Understand that open source tools are widely used on both desktop and server environments.

### 1.3 Open Source Software and Licensing (Weight: 1)
Open communities and licensing Open Source Software for business

**Key Knowledge Areas:** 
- Open source philosophy
- Open source licensing models
- Free Software Fundation (FSF) and Open Source Instiative (OSI)

**Important Concepts & Terms:**
- **Open source philosophy**
  - Software should be freely available to use, study, modify, and distribute.
  - Collaboration and community-driven development.
- **Open source licensing**
  - **Copyleft** (Strong protection): **GPL** (GNU General Public License) - If you modify and distribute, you must release your changes under the same license.
  - **Permissive**: BSD, MIT, Apache - Very flexible; you can use the code in proprietary projects with fewer restrictions.
- **Key Organizations**:
  - **Free Software Foundation (FSF)**: Founded by Richard Stallman. Promotes "Free Software" (freedom to use, study, modify, distribute).
  - **Open Source Initiative (OSI)**: Focuses on the "Open Source" label and business-friendly licensing.
- **Common Licenses**:
  - GPL (Copyleft)
  - BSD/MIT (Permissive)
  - Creative Commons (for non-software content)
- **Exam Tips:**
  - Know the difference between **Copyleft** vs **Permissive**.
  - Understand that "Free Software" (FSF) and "Open Source Software" (OSI) are related but have slightly different philosophies.

### 1.4 ICT Skills and Working in Linux (Weight: 2)
Basic Information and Communication Technology (ICT) skills and working in Linux.

**Key Knowledge Areas:** 
-Desktop skills
Getting to the command line
Industry uses of Linux, cloud computing, and virtualization

**Important Concepts & Terms:**
- Desktop skills
  - Using a graphical user interface (GUI) - browsers, file managers, basic configuration
  - Privacy concerns (tracking, cookies, data collection)
  - Basic productivity tools (LibreOffice, web browsing)
- Getting to the command line
  - Opening a terminal/console
  - Basic navigation and command
  - Understanding that most server/admin work is done via command line
- Industry uses of Linux
  - Servers (web, database, file, email)
  - Cloud computing (AWS Azure, Google Cloud) mostly run Linux
  - Virtualization (KVM, VirtualBox, VMware)

**Exam Tips:**
- Know that Linux dominates the server and cloud space.
- Understand the difference between desktop Linux (Ubuntu, Mint) and server Linux (Ubuntu Server, RHEL).

## Topic 2: Finding Your Way on a Linux System (Weight: 9)

### 2.1 Command Line Basics (Weight: 3)
Basics of using the Linux command line.

**Key Knowledge Areas:** 
- Basic shell usage
- Command line syntax
- Variables
- Quoting

**Important Concepts & Terms:**
- **Shell:** The most common is **Bash** (/bin/bash).
- **Command line syntax**: *command [options] [arguments]*
  - Example: *ls -l /home*
- **Variables:**
  - Environment variables (e.g., *$PATH*, *$HOME*)
  - Setting variables: *VAR=value*
  - Exporting: *export VAR=value*
- **Quoting:**
  - Single quotes (' ') - literal, no expansion
  - Double quotes (" ") - allow variable expression
  - Backsticks or $() - command substitution

**Partial List of Commands/Utilities:**
- *echo*
- *history*
- *type*
- *export*
- *PATH* environment variable

**Exam Tips:**
- Know the basic command syntax: *command [options] [arguments]*
- Understand the difference between single and double quotes.
- Know what *$PATH* is and why it matters.
- Be able to explain the difference between shell variables and an environment variable.

### 2.2 Using the Command Line to Get Help (Weight: 2)
Running help commands and navigation of the various help systems

**Key Knowledge Areas:** 
- Man pages
- Info pages

**Important Concepts & Terms:**
- **Man Pages** (*man*): The standard pages for commands.
  - **Usage:** *man ls*
  - **Navigation:** Space = page down, b = page up, q = quit
  - **Sections:** 1 = user commands, 5 = config files, 8 = admin commands
- **Info Pages** (*info*): more detailed, hyperlinked documentation (GNU style).
  - **Usage:** *info ls*
- **Other Help Methods:**
  - *command --help* (quick summary)
  - */usr/share/doc/* directory (additional documentation)

**Partial List of Commands/Utilities:**
- *man*
- *info*
- */usr/share/doc/*
- *locate* (for finding files)

**Exam Tips:**
- Know how to use *man* and *info*.
- Understand that *man* si the most common help system. 
  
### 2.3 Using Directories and Listing Files (Weight: 2)
Navigation of home and system directories and listing files in various locations

**Key Knowledge Areas:** 
- Files and directories
- Hidden files and directories
- Home directory
- Absolute and relative paths

**Important Concepts & Terms:**
- **Files vs Directories**
- **Hidden files:** Start with a dot (e.g., *.bashrc*, *.hiddenfile*)
- **Home Directory:** Represented by *~* or *$HOME*
- **Absolute Path:** Starts from root (*/home/usr/file.txt*)
- **Relative Path:** Relative to current location (*../file.txt* or *Documents/report.txt*)
  
**Important Commands:**
- *ls* (list files)
  - *ls -l* (long format)
  - *ls -a* (show hidden files)
  - *ls -la* (long + hidden)
- *cd* (change directory)
  - *cd* ~ or *cd* (go home)
  - *cd ..* (parent directory)
  - *cd /* (root directory)

**Exam Tips:**
- Know the difference between absolute and relative paths.
- Understand that *.* = current directory, *..* = partent directory
- *ls -a* is important for seeing hidden files.

### 2.4 Creating, Moving, and Deleting Files (Weight: 2)
Create, move, and delete files and directories under the home directory.

**Key Knowledge Areas:** 
- Files and directories
- Case sensitivity
- Simple globbing

**Important Concepts & Terms:**
- **Case Sensitivity:** Linux is case-sensitive (*File.txt* &#8800; *file.txt*)
- **Flobbing** (wildcards)
  - \* = any characters
  - ? = single characters
  - Example: ls \*.txt (all .txt files)

**Key Commands:**
- *touch* - Create empty file or update timestamp
- *mkdir* - Create directory
- *rmdir* - Remove empty directory
- *rm* - Remove files/directories
  - *rm -r* Recurisve (for directories)
  - *rm -f* Force (no confirmation)
- *cp* - Copy files/directories
- *mv* - Move or rename files/directories

**Exam Tips:**
- Know when to use *rm -r* vs *rmdir*
- Understand that *mv* can both move and rename
- Be careful with *rm* - no recycle bin!

## Topic 3: The Power of the Command Line (Weight: 9)

### 3.1 Archiving Files on the Command Line (Weight: 2)
Archiving files in the user home directory.

**Key Knowledge Areas:** 
- Files and directories
- Archives and compression

**Important Concepts & Terms:**
- **Archiving:** Combining multiple files into one file (tar)
- **Compression:** Reducing file size (gzip, bzip2, xz, zip)

**Key Commands:**
- *tar* - Teh main archiving tool
  - *tar -cvf archive.tar files...* (Create)
  - *tar -xvf archive.tar* (Extract)
  - **Common options:**
    - *-c* (create)
    - *-x* (extract)
    - *-v* (verbose)
    - *-f* (file)
    - *-z* (gzip)
    - *-j* (bzip2)
- **Compression tools:**
  - *gzip* / *gunzip*
  - *bzip2* / *bunzip2*
  - *xz*
  - *zip* / *unzip*

**Exam Tips:**
- Know the most common *tar* options (*-czvf*, *-xzvf*)
- Understand the difference between archiving and compression.
  
### 3.2 Searching and Extracting Data from Files (Weight: 3)
Search and extract data from files in the home directory

**Key Knowledge Areas:**
- Command line pipes
- I/O redirection
- Basic Regular Expressions using (., [], *, and ?)

**Important Concepts & Terms:**
- **Pipes(|):** Send output of one command as input to another
  - Example: *ls -l | grep ".txt"
- **I/O Redirection:**
  - \> : Redirect output to a file (overwrite)
  - \>> : Redirect output to a file (append)
  - < : Redirect input from a file
- **Basic Regular Expressions** (with *grep*)
  - . = any single character
  - \* = zero or more of the previous character
  - ? = zero or one of the previous character
  - [ ] = character class (e.g., [a-z])

**Key Commands:**
- *grep* - Search for text patterns
- *less* / *more* - View files one page at a time
- *cat* - Concatenate and display files
- *head* - Show first lines
- *tail* - Show last lines
- *sort* - Sort lines
- *wc* - Word count

**Exam Tips:**
- Master *grep* with basic regex - very common on the exam.
- Know the difference between > and >>

### 3.3 Turning Commands into a Script (Weight: 4)
Turning repetitive commands into simple scripts.

**Key Knowledge Areas:**
- Basic shell scripting
- Awareness of common text editors (vi and nano)

**Important Concepts & Terms:**
- **Shebang** (#!/bin/bash): First line of the script that tells the system which interpreter to use.
- **Variables:** *NAME="value"* and *$NAME* to use it.
- **Arguments:** $1, $2, etc. (positional parameters).
- **For Loops:** Basic iteration.
- **Exit Status:** $? (0 = success, non-zero = error)

**Key Commands / Tools:**
- Text Editors:
  - *nano* - Beginner-friendly
  - *vi* / *vim* - Powerful but steeper learning curve 

**Basic Script Structure Example:**
#!/bin/bash
\# This is a comment

NAME="World" \
echo "Hello $NAME"

\# Simple loop
for i in 1 2 3; do \
    echo "Number $i" \
done

**Exam Tips:**
- Know the shebang line.
- Understand how to make a script executable (*chmod +x script.sh*)
- Be able to read simple scripts with variables and loops.

## Topic 4: The Linux Operating System (Weight: 8)

### 4.1 Choosing an Operating System (Weight: 1)
Knowledge of major operating systems and Linux distributions.

**Key Knowledge Areas:**
- Differences between Windows, OS X, and Linux
- Distribution life cycle management

**The following is a partial list of the used files, terms, and utilities:**
- GUI versus comand line, desktop configurations
- Maintenance cycles, beta, and stable

### 4.2 Understanding Computer Hardware (Weight: 2)
Familiarity with the components that go into building desktip and server computers

**Key Knowledge Areas:**
- Hardware

**The following is a partial list of the used files, terms, and utilities:**
- Motherboards, processors, power supplies, optical drives, peripherals
- Hard drives, solid state disks, and partitions, /dev/sd*
- Drivers

### 4.3 Where Data is Stored (Weight: 3)
Where various types of information are stored on a Linux system.

**Key Knowledge Areas:**
- Programs and configuration
- Processes
- Memory addresses
- System messaging
- Loggin

**The following is a partial list of the used files, terms, and utilities:**
- ps, top, free
- syslog, dmesg
- /etc/, /var/log/
- /boot/, /proc/, /dev/, /sys/

### 4.4 Your computer on the Network (Weight: 2)
Querying vital networking configuration and determining the basic requirments for a computer on a Local Area Network (LAN).

**Key Knowledge Areas:**
- Internet, network, routers
- Querying DNS client configuration
- Querying network configuration

**The following is a partial list of the used files, terms, and utilities:**
- route, ip route show
- ifconfig, ip addr show
- netstat, ss
- /etc/resolv.conf, /etc/hosts
- IPv4, IPv6
- ping
- host

## Topic 5: Security and File Permissions (Weight: 7)

### 5.1 Basic Security Identifying User Types (Weight: 2) 
Various types of users on a Linux system.

**Key Knowledge Areas:**
- Root and standard users
- System users

**The following is a partial list of the used files, terms, and utilities:**
- /etc/passwd, /etc/shadow, /etc/group
- id, last, who, w
- sudo, su


### 5.2 Creating Users and Groups (Weight: 2)
Creating users and groups on a Linux system. 

**Key Knowledge Areas:**
- User and group commands
- User IDs

**The following is a partial list of the used files, terms, and utilities:**
- /etc/passwd, /etc/shadow, /etc/group, /etc/skel/
- useradd, groupadd
- passwd

### 5.3 Managing File Permissions and Ownership (Weight: 2)
Understanding and manipulating file permissions and ownership settings.

**Key Knowledge Areas:**
- File and directory permissions and ownership

**The following is a partial list of the used files, terms, and utilities:**
- ls -l, ls -a
- chmod, chown

### 5.4 Special Directories and Files (Weight: 1)
Special directories and files on a Linux system including special permissions.

**Key Knowledge Areas:**
- Using temporary files and directories
- Sysbolic links

**The following is a partial list of the used files, terms, and utilities:**
- /tmp/, /var/tmp/, and Sticky Bit
- ls -d
- ln -s













<!-- End of File -->





