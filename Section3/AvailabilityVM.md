Welcome back.
Starting this step, let's look at a very, very important aspect of deploying applications to the Cloud,

which is Availability.
What is Availability? Are the applications available when the users need them?
Availability is a percentage of time an application provides the operations that are expected of it.
A good example of availability is 99.99% availability.
This is also called four 9's availability. To understand the impact of four 9's availability,

What is Premium SSD or Ultra Disk?
We talked about the fact that virtual machines can be attached with disks.
There are different types of disks which are present.
Premium SSD Ultra Disk, Standard SSD, Standard HDD, and based on the disk which is attached, the availability guarantee from Azure for your virtual machine varies. If you are attaching Premium or Ultra Disk, it's 99.99%.
If you are attaching Standard SSD, the availability goes down, 99.5.
If you are attaching standard HDD, Hard Disk Drive,
then it goes down even further, 95%.

Let's quickly see where you can see these disk types. You can go to Add, Virtual machine
and go to Disks, and this is where you can see the different disk types.
So, right now, we are making use of Premium. You can also use Standard SSD, Standard HDD as well.

As it says in here, Ultra Disk option is only available when we are making use of Availability Zones.
We would look at how you can use Availability Zones a little later when we are playing with Scale sets.

Now, if you'd want to further increase the availability for your Azure VM, what you would need to
do is to create two or more instances in the same Availability Set.
So, if you create two VMs in the same availability set, the availability increases from
99.9% to 99.95%. While the increase looks small, it is very, very important when it comes to online applications.

So, if you'd create two instances in an availability set, you get higher availability.
But what is an availability set?
Where can you configure it?
Availability Set is nothing but a logical grouping of virtual machines.
Instead of creating single virtual machine, you'd want to create a logical group of a number of virtual
machines.
And, whenever we are talking about availability sets, there are two important concepts;\
Fault domains and Update domains.
Fault domains are nothing but a group of VMs sharing a common power source and network
switch. If I have two VMs and both the VMs are deployed to the same fault domain,
what would happen if the power source goes down?
Both the VMs would be down. So, for a higher availability, you would want to distribute your VMs across different fault domains.

You don't want all your VMs to share the same common power source and networks switch. The other important concept is Update domains. These are group of VMs that are updated or rebooted at the same time.
Any maintenance that is done on all the VMs in a single update domain, the maintenance would be done at then same time.
If I have 10 VMs and all the 10 VMs are in the same update domain, what would happen?
All of them would be updated at the same time, they might be rebooted and that would cost downtime in
the application and I don't want that as well.

I would want to distribute the VMs across different update domains as well.
So, whenever we are creating VMs, we'd want to distribute them across fault domains and across update domains, so that all of them don't go down at the same time.

And, the way you can do that is by making use of an availability set. Where do you create an availability
set?
Let's go back to Basics when we create a virtual machine and let's scroll down.
And over here, you have availability options and this is where you have the option to create a availability set.

So, I can go here and say I would want to create an availability set.
You can go ahead and create a new availability set right here.
So, you can say, I'd want to create a new availability set and you can configure the name of the availability set, and how many different fault domains and update domains you would want to make use of.

So, if I would want to create 10 VMs, probably I would choose five update domains and two different fault domains.
If you have one fault domain and one update domain, then your availability will be low.
However, if you increase the default domains to either two or three and increase the number of update domains, let's say I would want five update domains or ten update domains, then the chances that all the VMs would go down at the same time, will go down substantially.

So, whenever you're creating a virtual machine, you can associate it with a availability set. If you have
multiple virtual machines which are associated with the availability set, then the availability set
would ensure that those virtual machines are distributed across different fault domains and update domains.

In summary,
if you'd want high availability, you'd want to create multiple instances.
If you create multiple instances in the same availability set, you get 99.95%
availability.

If you'd create the instances in two or more availability zones, then you'd get up to
99.99% availability.
