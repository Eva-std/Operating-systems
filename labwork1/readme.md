> Performed by student  
> KSM-43b group  
> Адаменко Є. В.  

<h1 align="center">Lab work №1</h1>

## Pre-lab assignment
### Task 1
#### Прочитайте короткі теоретичні відомості до лабораторної роботи та зробіть невеликий словник базових англійських термінів з питань класифікації віртуальних середовищ
- Hypervisor - a software that allows multiple operating systems to run simultaneously on the same physical hardware
- Type 1 hypervisor - a hypervisor that runs directly on hardware with no underlying host OS support; must perform all functions itself
- Type 2 hypervisor - a hypervisor that runs on top of a host operating system, using its file system to create processes and store files
- Guest OS - an operating system running inside a virtual machine, on top of the hypervisor
- Host OS - the underlying operating system on which a type 2 hypervisor runs
- Binary translation - a technique of translating blocks of code on the fly, storing them in an internal cache, and reusing them if executed again, used to improve virtual machine performance
- Machine simulator - an intermediate virtualization approach that uses binary translation to run guest OS processes on top of a host operating system
<br>

### Task 2.1 
#### Охарактеризуйте поняття «гіпервізор». Які бувають їх типи?
##### Hypervisor (originally called "virtual machine monitor") - a software that allows multiple operating systems to run simultaneously on the same hardware. 
##### Types of hypervisors:
 - A type 1 hypervisor   
 - A pure type 2 hypervisor   
 - A practical type 2 hypervisor
<br>

### Task 2.2 
#### Перерахуйте основні компоненти та можливості гіпервізору VirtualBox.
##### VirtualBox - is a free, open-source type 2 hypervisor developed by Oracle.  
Main components: 
- Guest Additions - special drivers installed in the guest OS to improve performance and integration
- Virtual Disk - a virtual hard drive stored as a file
- Virtual Network Adapter - a virtual network interface card
- Snapshot Manager - a manager for saving system state snapshots
- Extension Pack - an add-on package for additional features
##### Main features:
- Running multiple operating systems simultaneously (Windows, Linux, macOS, Solaris)
- Creating snapshots - saving the state of a VM at any point in time
- Shared folders between the host and guest OS
- Screen recording of the virtual machine
- VBoxManage command-line interface for managing VMs without a GUI
<br>

### Task 4
#### Пройдіть тестування у курсі NDG Linux Essentials Chapter 02 Exam
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork1/task4.png?raw=true)
<br>
<br>

## Lab steps
### Task 2 - Дайте відповіді на наступні питання  
#### 2.1 Перерахуйте етапи для розгортання операційної системи на базі віртуальної машини VirtualBox.
##### To deploy an operating system on VirtualBox, follow these steps:
1. Download and install VirtualBox on the host OS
2. Create a new virtual machine
3. Allocate RAM for the virtual machine
4. Create a virtual disk (VDI file)
5. Attach the ISO image to the virtual machine
6. Complete the guest OS installation wizard
<br>

#### 2.2 Чи є якісь апаратні обмеження при встановленні 32- та 64-бітних ОС?
##### Yes, there are hardware limitations when installing 32-bit and 64-bit OS:
##### 32-bit OS:
- Max 4 GB RAM
##### 64-bit OS:
- Requires a 64-bit processor
- Requires hardware virtualization enabled in BIOS/UEFI
- Supports more than 4 GB RAM
<br>

#### 2.3 Які основні етапи при встановленні OS Linux в текстовому режимі?
##### The main stages of installing Linux OS in text mode are:
1. Boot from installation media
2. Select installation language and keyboard layout
3. Configure network (like host name)
4. Set date and time (timezone)
5. Select software packages to install
6. Install the bootloader
7. Set root password and create a user account
8. Reboot the system
9. First login via text mode terminal
<br>

#### 2.4 Яким чином можна до установити графічні оболонки Gnome та KDE в Linux, якщо вона вже встановлена в текстовому режимі (вкажіть необхідні команди та пакети)? 
##### GNOME for Ubuntu/Debian:
```
sudo apt update  
sudo apt install ubuntu-gnome-desktop
```
##### GNOME for Red Hat/CentOS/Fedora:
```
sudo dnf groupinstall "GNOME Desktop Environment"
```
##### KDE for Ubuntu/Debian:
```
sudo apt update
sudo apt install kde-plasma-desktop
```
##### KDE for Red Hat/CentOS/Fedora:
```
sudo dnf groupinstall "KDE Plasma Workspaces"
```
##### Start GUI after installing:
```
sudo systemctl start display-manager
```
##### Set GUI as default startup mode:
```
sudo systemctl set-default graphical.target
reboot
```
<br>

#### 2.5 Дайте коротку характеристику графічних інтерфейсів KDE та Fluxbox, що використовуються в різних дистрибутивах Linux 
##### KDE (K Desktop Evvironment) - is a full-featured, visually rich desktop environment based on the Qt framework. It is highly customizable and includes a complete suite of built-in applications such as a file manager, browser, and text editor. KDE requires relatively high system resources. It's interface is similar to Windows, making it easy for beginners.

##### Fluxbox - is an extremely lightweight window manager based on Blackbox. It provides a minimal interface consisting of only a taskbar and a right-click menu, making it ideal for old hardware or embedded systems. Fluxbox has no built-in applications like KDE, for example and is configured through text configuration files, making it more suitable for experienced Linux users.
<br>
<br>

## Сontrol questions
### 1. Порівняйте гіпервізори типу 1 та типу 2, яка між ними відмінність та сфера їх застосування?
##### The real distinction between a type 1 hypervisor and a type 2 hypervisor is that a type 2 makes use of a host operating system and its file system to create processes, store files, and so on. A type 1 hypervisor has no underlying support and must perform all these functions itself. 
##### Scope of application:
1. Type 1 hypervisor:
   - Enterprise servers and data centers
   - Cloud computing platforms
   - Critical business infrastructure
   - Environments where performance and stability are a priority
2. Type 2 hypervisor:
   - Personal computers and laptops
   - Software development and testing
   - Education and learning environments
   - Running multiple OS simultaneously on a single personal machine
<br>

### 2. Розкрийте поняття «GNU GPL», яка його основна концепція?
##### GNU GPL (General Public License) - is a free software license created by Richard Stallman in 1989 as part of the GNU project. The main concept - "copyleft": software can be freely used, source code can be freely viewed, software can be freely modified, modified software must be distributed under the same GPL license/
<br>

### 3. В чому суть програмного забезпечення з відкритим кодом?
##### Open source takes a source-centric view of software. The open source philosophy is that you have a right to obtain the software source code and to modify it for your own use. Linus made the source programming code freely available, allowing others to join in and shape this fledgling operating system. People took the source, made changes, and shared them back with the rest of the group, greatly accelerating the pace of development, and ensuring mistakes from other operating systems were not repeated.
<br>

### 4. Що таке дистрибутив?
##### A distribution - is a complete package that combines the Linux kernel, system tools, and a set of applications bundled together into a ready-to-use operating system. The distribution includes tools that take care of setting up the storage, installing the kernel, and installing the rest of the software. The full-featured distributions also include tools to manage the system and a package manager to help you add and remove software after the installation is complete.
<br>

### 5. Які задачі системного адміністрування можна реалізувати на базі ОС Linux?
##### Linux-based system administration tasks:
- User and group management
- File system and storage management
- Network configuration and monitoring
- Security and firewall management
- Backup and recovery
- Server configuration (web, mail, DNS, FTP)
- Process and resource monitoring
<br>

### 6. Як пов'язані між собою ОС Android та Linux?
##### Android, sponsored by Google, is the world's most popular Linux distribution. It is fundamentally different from its counterparts. Android uses the Dalvik virtual machine with Linux, providing a robust platform for mobile devices such as phones and tablets.
<br>

### 7. Основні можливості та сфера використання Embedded Linux?
##### Main features of Embedded Linux:
- Support for a wide range of hardware architectures
- Ability to run with minimal RAM (from 2 MB)
- Real-time data processing
- Remote management and updates
- Support for various file systems
- Network connectivity
- Graphical interface support
- High level of security and access control
<br>

### 8. Яким чином можна змінити типу завантаження Linux: в текстовому режимі (3 рівень) або графічному (рівень 5)? Чим відрізняються режими CLI та GUI?
##### In a GUI, applications are presented in windows that can be moved and resized. There are menus and tools for navigation. CLI is a text-based interface that relies primarily on keyboard input. Everything the user wants to do is accomplished by typing commands rather than clicking on icons.
##### Set text mode (runlevel 3):
`sudo systemctl set-default multi-user.target`
##### Set graphical mode (runlevel 5):
`sudo systemctl set-default graphical.target`
<br>

## Conclusions
##### During the completion of lab. work №1, I studied hypervisors and their types, namely Type 1 and Type 2, and learned about their differences and areas of application. I learned how to install and run Linux on Windows using VirtualBox, and how to work with Linux in a virtual environment. Also I learned how to switch between text (CLI) and graphical (GUI) modes of the operating system, as well as how to change Linux boot levels. Using the Cisco course, I familiarized myself with the main types of modern operating systems — Windows, macOS and Linux, and studied their capabilities, functions and differences. I also learned about the main Linux distributions (Ubuntu, Red Hat, Debian, Android, etc.) and the concept of open source software (GNU GPL).
