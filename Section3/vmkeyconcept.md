Welcome back.

In the last step, we were able to create a virtual machine and we were able to SSH into it.
Let's quickly look at some of the important concepts that are related to Azure Virtual Machines.

The first important concept is that of a Image.
Image helps you to choose the right operating system and the software for your virtual machine.
So, the image is the one which decides what operating system is used on the virtual machine.

The second important concept is that of a Virtual Machine Family. What is a Virtual Machine Family?
There might be different kinds of applications that you would want to run on your virtual machine.
You might have a General purpose web application or you might be using the virtual machine as a cache.
If you are using virtual machine as a cache, you need a lot of memory. In that kind of situation,
you would want to make use of Memory Optimized instances.
You might be running a High-Performance Compute workload. In those kind of situations,
you want to make use of a HPC.
You might be running a graphics application on your VM.
In those kind of situation, you might want to choose a GPU-based hardware.
So, a VM Family is the thing that helps us to choose the right family of hardware for your specific application that we'd want to run on the virtual machine.

To your virtual machines, you can also attach virtual disks.
This is very, very similar to attaching a hard disk to your laptop or computer.
Where is the disk that is attached to our virtual machine?
