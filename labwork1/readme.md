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

### Task 2.1 
#### Охарактеризуйте поняття «гіпервізор». Які бувають їх типи?
##### Hypervisor (originally called "virtual machine monitor") - a software that allows multiple operating systems to run simultaneously on the same hardware. 
##### Types of hypervisors:
 - A type 1 hypervisor   
 - A pure type 2 hypervisor   
 - A practical type 2 hypervisor

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

### Task 4
#### Пройдіть тестування у курсі NDG Linux Essentials Chapter 02 Exam
![alt next](https://github.com/Eva-std/Operating-systems/blob/main/labwork1/photos/task4.png?raw=true)
