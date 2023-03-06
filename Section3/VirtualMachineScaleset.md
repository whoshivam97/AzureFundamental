Welcome back.

Starting this step, let's look at Virtual Machine Scale Sets. How do you simplify the creation and management of multiple virtual machines? That's where we would go for virtual machine scale sets.

This allows you to create and manage a group of Azure Virtual Machines.
This provides high availability for your applications. In the previous step,
we saw that if I create multiple VMs, I get higher availability.
If I create multiple VMs across multiple availability zones, I get even higher availability.

Virtual machine scale sets also allows you to add a load balancer.
So, if you have multiple Azure VMs, if you have your application deployed to them, you'd want to be
able to load balance between those instances.
Virtual machine scale sets also helps you to create a load balancer.
It also helps you to distribute VM instances across multiple availability zones.

As we discussed earlier, not all regions have multiple availability zones. Wherever you have multiple availability zones, you can use a scale set to distribute your VM instances across multiple availability zones.

Virtual machine scale sets also supports manual scaling and auto scaling.
Let's have five instances right now.
I can increase it to 10, 15. I can do that manually.
The other option I also have is auto scaling.
Based on the number of requests which are coming in, I can increase the number of instances automatically.
You can create up to thousand virtual machine instances in a single scale set.
