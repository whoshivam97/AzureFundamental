Welcome back. In this step,
let's explore a few more features around Azure Virtual Machines. Static IP address,what is the need for a static IP address?

Let's go over to Virtual machines.
One of the important things that you need to understand is public IP addresses are not free.
Every public IP address that you create has a charge associated with it.

If you want to see the status of the things which you are doing right now, you can go to notifications.
You can go in here and see what are the different events which are happening in here.
All these events are coming in from something called an activity log.

If you don't want the public IP address of a virtual machine to change, in those kind of situations,
you can assign a static IP address.
How can you do that?
Let's see how you can do that when creating a new virtual machine. Let's say Add Virtual machine
and over here, go over to Networking
and this is where you can actually create a new public IP. So, let's say create new IP.

When you create a static IP address, that IP address will not change.
public IP addresses are of two kinds; Dynamic and Static. Dynamic changes
every time you stop and start. Static remains constant.
So, a static IP address is a fixed IP address that can be assigned to your VM.

Important thing to remember is public IP addresses, whether they are Dynamic or Static, they are charged
per IP address per hour.
So, if you have unused IP addresses, the best practice is to release them as soon as possible.

The next important feature that we'll be looking at is Azure Monitoring. What is Azure Monitoring
used for?
Let's pick up the second VM.
Let's say unsaved edits will be discarded, that's ok. That's ok. Over here, if you go to Monitoring,
you can see a lot of metrics around that specific virtual machine.
Let's go to 6 hours and you can see the CPU usage over a period of time.
You can see the Network.
You can see the Network usage over here. You can see the Disk bytes, Disk operations. So, you can see
all the metrics around your VMs. Where are these metrics coming in from?
These metrics are coming in from Azure Monitor.
The other option you have to see the metrics is to go to Monitoring.

So, once inside the virtual machine, you can go into Monitoring and also go to Metrics.
Over here, you can also create charts and visualize all the metrics. Let's say I would want to create a CPU
Credits Consumed chart. I can say CPU Credits Consumed and look at the chart for it. So, over here, you can create your own charts, add in your own metrics, and visualize them.

So, Azure Monitoring provides monitoring for your Azure Virtual Machines.
A little later in the course,

we will also learn that Azure Monitoring can monitor a variety of Azure services.
Most of the Azure services can be monitored by using Azure Monitoring.

The other important feature of a virtual machine is something called Dedicated Hosts.
What are Dedicated Hosts?
Dedicated Hosts are physical servers which are dedicated to one customer.
Typically, whenever you look at Azure on a single host, there would be multiple virtual machines that
are created and each of these virtual machines belong to different customers.
Azure ensures that these virtual machines are isolated from each other.
However, underneath the hood, they are still sharing the same hardware.
They're still sharing the same host.
Sometimes there are compliance needs where you need to deploy your applications only on dedicated hardware.
In those kind of situations, you can go for Dedicated Hosts.

Where can you see Dedicated Hosts? You can type in Dedicated
Hosts. Go to Marketplace and select Dedicated Hosts
and this is where you can actually create a Dedicated Host. So, you can create a Dedicated Host.

All the virtual machines on this host are guaranteed to be belonging to you. You can create a Dedicated
Host and then you can create virtual machines on this Dedicated Host.

Another interesting feature in Azure Virtual Machines, enables you to create cheaper temporary instances
for non-critical workloads.
Let's say I have a batch job.
Let's say it's crossing 10000 records.
Let's say it processes them in batches of hundred.
Let's say this is not a very essential batch job.
I can run it within the next couple of months.
For me, the priority with this batch job is to run it as cheaply as possible.
If you have batch jobs like this which are fault-tolerant, basically, if there is a failure, you'll be able to quickly recover from it.

If you have fault-tolerant batch jobs, you can use Azure Spot instances to be able to run them.
How can you create Azure Spot instances?
Let's go to virtual machine
and let's add a Virtual machine, and over here, you can go in and say, I would want to create a Spot
instance.
So, Azure Spot offers unused Azure capacity at a discounted rate versus pay as you go prices.
Very, very important thing is workload should be tolerant to infrastructure loss as Azure may recall capacity for these workloads.
As it says in here, Azure Spot VMs allow you to take advantage of unused capacity at significant
cost savings.

The most important thing that you need to remember is there is no guarantees associated with this Spot
Virtual Machines.
At any point in time, Azure might want the virtual machine back and it would give you a 30 second
notice.
Another option that Azure Virtual Machines provides to help you manage your costs is to reserve
compute instances ahead of time.
You can go ahead and reserve VM instances ahead of time for one or three years.
You can go in here and say, I would want to create a Reservation. So, you can go and create a reservation
and say I would want to add a reservation. You can see that you can add reservations for a variety of services.
There are a lot of other services that we will be talking about a little later.

Reserved VM instances provide a significant discount over pay as you go VM prices.
This allow you to pre-purchase the base costs of your VM usage for a period of one or three years.
You can reserve for one or three years.

Static IP addresses allow you to give a fixed IP address to your VM.

Azure Monitoring helps you to monitor the metrics around your virtual machine.

If you'd want a physical server which is dedicated to just one customer, you'd go for Dedicated Hosts.

If you'd want to manage your cost with your virtual machines, you have couple of options, you have fault-tolerant workloads, then you can go for Spot Instances.

You would want to reserve instances ahead of time, then you can go for Reserved VM instances.

Over here, you can reserve instances for one or three years.
