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
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork1/photos/task4.png?raw=true)
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
##### 
