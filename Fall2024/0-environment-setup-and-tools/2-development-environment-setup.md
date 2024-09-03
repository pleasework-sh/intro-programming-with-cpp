# Development Environment Setup

## The Virtual Machine
One of our first assignments is going to be setting up our development environment. 

For consistency purposes we will be using Ubuntu (for Windows Hosts and Intel Mac Hosts) or Kali Linux (for Apple Silicon m-chip hosts). We will set up virtual machines for our development environments. 

> [!NOTE]
> This assumes that you have no prior knowledge of any sort of Linux operating system. This also assumes you are running a Windows or MacOS host, which is typical for new students. If you are already a Linux power user, feel free to JMP straight to the programming portion of the course. If this is the case for you, you are probably already exposed to the majority of the concepts taught here and you just need this course for college credit. If this is the case, feel free to reach out to me so we can accelerate you through the course if you wish. 

> [!NOTE]
> For more experienced folk, you might be wondering, why are we using Kali Linux instead of Ubuntu on Apple Silicon Macs for this course? Kali Linux is a penetration testing distribution, it's not really meant for software development. The reason I chose Kali Linux here is because the ease of installation would be a teeny bit easier - only because it already came with a GUI installed as opposed to the official Ubuntu Server ARM-based images, which don't have a GUI installed. Of course, right after writing this I found that there are Ubuntu Desktop ARM-based images that DO come with a GUI installed, but it was too late to change the assignment at this point. 

Typically you are not exposed to virtual machines in an intro programming course, but another goal of the course is to introduce you to tools that you will have roughly a 90% chance of running into again. By introducing you to these tools early and having you struggle with them, you will be more knowledgeable and ahead of some of your peers. For many of us, the end goal of our degrees is to get a job in the industry, so we shall practice with industry tools. (Full disclaimer, every company may have a different set of tools that you may use as a software developer - some software engineers may not use virtual machines at all. But, using Linux virtual machines will help you gain exposure to the command line, which you will definitely run into in your career).

In beginner terms, a virtual machine (VM) is like emulating a "computer in your computer." For anyone who has emulated retro games on their PC before, it's a similar principle. VMs are great because you can separate your development work from whatever other work you are doing on your HOST machine (whatever machine you are running the VM on). 

Please review the following articles about virtual machines to learn more about them:
- [What is a virtual machine?(VM) - Azure](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-a-virtual-machine)
- [What is a Virtual Machine? - RedHat](https://www.vmware.com/topics/virtual-machine)

The software we use to run our virtual machine is a called a **hypervisor**. There are two types, **Type 1**, AKA bare metal hypervisors - which typically run on dedicated servers. Type 1 hypervisors include ProxMox and VmWare VSphere. Bare metal hypervisors run directly on the computer hardware and are used on machines that are completely dedicated to virtualization.

Contrast this with **Type 2** hypervisors which are the kind that we will be using in the course. Type 2 hypervisors are just another application installed on your computer operating system, whether that be Windows or MacOS. We use Type 2 hypervisors on machines that might be dedicated to functions other than virtualization, such as our personal computers.

Virtualization runs the world. By running virtual machines, we can make the most efficient use of our computer hardware. What we refer to "the cloud" is for the most part, a bunch of virtual machines running on servers in highly secured data centers.

## The hypervisors we will be using and VM Setup
The hypervisor we will be using depends on our host OS. 

For Windows / Apple Intel users, we will be using VirtualBox. 

For Apple Silicon users (if you purchased your Macbook in 2020 or later, it is most likely an Apple Silicon chip), we will be using UTM. 

Please download and install the appropriate hypervisor for your operating system.

See the download links below: 
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- [UTM](https://mac.getutm.app/)

# For setting up your VM, please refer to the assignment in the course in D2L

## Integrated Development Environments (IDEs) (and what we will be using instead)

Integrated Development Environments (IDEs) are great because they do so many helpful things like syntax checking, compiling, debugging and overall making our lives as programmers easier.

So we won't be using them in this course! 

I find that when students start off programming in an IDE like Visual Studio they often get confused because a Visual Studio project creates a lot of extra files and folders specific to Visual Studio. Additionally, it doesn't train you to look for syntax errors if something goes wrong in your code because the IDE does it for you. 

Instead, we will be using a plain text editor. 

If you're feeling spicy, try using vim. Otherwise we will be using gedit, which has a simple GUI. We will be going more in depth in the next reading. 