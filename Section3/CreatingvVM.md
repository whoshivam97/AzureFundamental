Let's get started with the hands-on for Azure Virtual Machines where we would create a few Virtual Machine instances and play with them.

Let's get started.
If you go to portal.azure.com and sign in with the userId and password that we created earlier,
you would see a page like this.
It says, Welcome to Microsoft Azure.

There are a number of services which are present in Azure.
You can click this icon which is present on the left top corner and you'd be able to see a wide variety

of services which are present in Azure.

Let's not really worry about all of them. For now,

let's focus on virtual machines.

What you can do is either click Virtual machines in here or you can also type in Virtual Machines.

So, I'd type in Virtual Machines and go in there.

What do we want to do is to create a virtual machine. So, I'll go ahead and say Add and select virtual machine

option from here.

So, we would want to add a virtual machine.

The page would take a couple of seconds to load.

Now, let's see what is involved in creating a virtual machine.

Right now, we are in the Free Trial, that's what is called a Subscription and in the Free Trial subscription,

we would want to create a resource group.

A virtual machine is a resource, a database is a resource. There might be a number of resources which

are related to a single project or a single business unit. You'd want to group them in some way.

In Azure, the way you can group them is by creating a resource group.

If you have a virtual machine, a database, and maybe a queue, which is related to the same project,

you can create a resource group and you can put all these resources under the same resource group.

For now, what we'd do is, we would create a new resource group

and I will call this compute-rg.

Right now, we are exploring all the compute services. So, I would actually put it as compute-rg

and I'll say, ok. So, we are creating a new resource group, compute-rg.

The next thing that we'd need to configure is the name for our virtual machine.

I'll call this, my-first-vm. Now, after that there are three very important choices that we would typically

need to make.

Number one is region.

Which region do you want to deploy this virtual machine to?

Earlier we talked about the fact that Azure offers sixty-plus regions and you can deploy virtual machines

to any of those regions.

You can click this dropdown and choose which region you would want to deploy your virtual machine

to.

I would recommend you to choose the default one, which is (US) East US.

The second important choice that you need to make is what operating system do you want on your virtual

machine.

You select the operating system by choosing the image.

There are a wide variety of images which are offered.

You can see Ubuntu, Red Hat Linux, Windows Server.

There are a wide variety of operating systems which are supported.

What I'd recommend you to do is, to choose the default one which is suggested, which is Ubuntu Server

18.04 Long Term Support.

The third important decision that you would need to make when creating a virtual machine is the size

of the virtual machine.

How big should your virtual machine be?

There are a wide variety of sizes which are present.

Once you click the dropdown, you can choose the sizes which is recommended in here or you can say

see all sizes and look at a wide variety of VM sizes which are offered by Azure.

If you do a Google for azure free tier and click the link which comes up in here, this is what we use

to create the Azure account earlier.

If you scroll down, you can see products which are free for twelve months, up to a monthly limit. Over here,

you can see that under Linux Virtual Machines, you have 750 hours free of B1S Standard tier.

So, what we'll do is, we'll use this machine type because this comes free for us. So, let's go ahead there and select

a VM size.

You can type in B1S and then this is filtered down or you can even scroll and choose there, if you

are able to select one of the rows and then go and select B1S, it's in here.

You can see that B1s has one vCPU and one GiB of RAM and you can have up to two Data disks

which are attached with it.

For all our demos, that should be more than sufficient.

So, let's make use of B1S and I'll say Select.

So, the three important choices that we have made until now are one, the region, where do you want to run the virtual

machine.

Number two is image,

what OS do you want to make use of.

Number three is the size,

what is the hardware you'd want to make use of to run your virtual machine,

right now which was one vCPU and one GiB of memory. Now,

over here, if you further scroll down, you can choose how you'd want to authenticate yourself when you're trying

to access the virtual machine.

What I would recommend you to do is to do SSH public key.

So, let's use SSH public key.

I'll leave the Username at default.

What I would do is, I would generate a new key pair. So, we will generate a new key pair and let's have the key pair

name as my-first-VM_key. That's the default which is suggested.

If you scroll down further, you can also configure what are the inbound ports which are allowed.

I'm creating a virtual machine,

what are the ports on which I can access the virtual machine from outside?

Right now you can see that by default, SSH on port 22 is allowed.

What I would want to do is to add one more port. So, I'll click the dropdown and I'll check HTTP

port.

What we want to do later is to install a web application on the specific virtual machine and therefore

I'd want to enable HTTP and SSH. So, we would want to be able to access this virtual machine on port 22,

that is SSH, and port 80, which is to access a web application and now,

we are all set to create our first virtual machine.

What we would do is, we would go ahead and say, Review and create.

There is a lot of advanced configuration that you can customize when you create a virtual machine.

Let's not worry about it. To start with,

let's focus on the basics and let's try and create a virtual machine. Whenever we create a resource,

Azure would validate our resource configuration and that's what is happening in the background right

now. It's running a final validation of our virtual machine configuration.

It says validation passed and now we can go ahead and create this virtual machine.

Once you click Create, you should see a pop up where you can actually download the private key.

We have created an SSH key and we can download the private key and store it.

So, let's download the private key. Make sure that you download it and have it in a safe place because

we would be making use of this file

in the next step. I would say Allow. I would want to download and this key is now downloaded into the

Download folder in my machine. A very important warning,

do not share that key pair with anybody, because anybody who has that key pair will be able to access your

virtual machine.

So, keep it private.

The creation of the virtual machine is right now in progress.

You can see that the deployment is right now in progress.

Let's wait for a few minutes and I'll see you in the next step.
