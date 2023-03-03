Earlier, when we talked about the cloud, we talked about the fact that you can "Go global" in minutes.
You can deploy applications to different parts of the world
within minutes, if you are using the Cloud.

Now, how can you do that?

The most important concepts that enable us to do that are Regions and Zones
and in this step, let's focus on understanding why we need Regions and Zones.

Let's take a simple example and discuss that further.

So, imagine that your application is deployed in a data center in London.
You have a corporate data center in the London region and you have an application deployed in there.

Let's say your users are distributed globally, what would be the challenges?

The number one challenge would be slow access for users from other parts of the world.
So, if I'm accessing this application, let's say, from Sydney or let's say I'm accessing it from Mumbai
or Chennai or New York, the application will be a little slow.
This is also called high latency. So, we will have high latency for users from other parts of the world.

Number two, let's imagine the scenario where this data center crashes
and because we just have one instance of the application, the application is no longer available.
So, the application goes down.
So, the application has low availability.

Now, think about this, what can we do to improve this situation?
Let's add one more data center in London, right.
So, I have one data center in London, I'll add one more.
So, we have Corporate Data Center 1 and Corporate Data Center 2.

Now, think about this, what were the challenges now?
Let's talk about the challenge one, slow access for users from other parts of the world. This challenge
still remains.
No change as far as challenge one is concerned. Challenge two, what if one data center crashes is solved,
why?
Because if one data center crashes, your application is still available from the other data center.
So, that's cool, right?

So, that's one challenge we made progress with.

However, what if the entire region of London is unavailable. So, if this entire region of London is
unavailable, what happens? Your application goes down.

Now we think a lot and come up with a better solution.

What do we do?

We add a new region.
We add a new region, Mumbai.
So, we have a London region, we have a Mumbai region, and each of these regions has two different data
centers. Now, think about our challenges.
Challenge one is partly solved.
At least the users who are nearer to Mumbai get faster access to the application.
Actually, you can completely solve the challenge one by adding deployments for your application in multiple regions around the world. So, you can add a deployment in Sydney, New York, and rest of the world, maybe somewhere in the Middle East, somewhere in Africa, somewhere in South America.

So, you can add deployments everywhere
and solve this challenge. Challenge two, what if one data center crashes? That is already solved.
What if entire region of London is unavailable, what would happen?
Your application is now served from Mumbai.
So, challenge three is now solved.
So, by having multiple regions and having multiple data centers in each of these regions, we can provide
high availability to the user.
The other thing which will also improve is the latency. Users who are nearer to each of these regions
can get faster access to these applications and that is the reason why each of the Cloud providers
provide concepts called Regions and Zones.

Welcome back.

In the previous step, we talked about the fact that setting up data centers in different regions around
the world is not easy and that's where all the cloud providers, including Azure, provide us with
regions all around the world. Azure provides sixty-plus regions around the world which is an ever-expanding list. There are new regions added in every year.
Azure is the Cloud provider which provides the most number of regions around the world.

Now, what is a region?
A region is nothing but a specific geographical location where we can host our resources.

You can decide,

I'd want to host my application in Mumbai region or I can say, I'd want to host my application in London
region or Sydney region. By having multiple regions around the world, Azure makes it very, very easy
for us to deploy applications to these regions.

The important advantage of having multiple regions around the world is High Availability.
If you deploy your application to multiple regions around the world, even if one of the regions is
down, you can serve the application from the other regions.

Number two is Low Latency.
You can serve users from the nearest region to them and therefore they get low latency.

Number three is Global Footprint.
A startup in India might be able to easily deploy applications to multiple parts of the world and therefore it can create global applications.

The last advantage is adherence to global regulations.
Different countries have different regulations.
For example, let's say, United States of America or USA
want the data related to all its citizens to reside only within their country.
In those kind of situations, we can create a region in US and store data related to US customers
only in that specific region.

So, regions help us achieve high availability, low latency, global footprint, and help us to adhere
to Government regulations.

What is the need for Zones?
How do you achieve high availability in the same region? That's where Availability Zones are very useful.
Azure provides multiple Availability Zones in some of the regions. Each Availability Zone is one or more
discrete data centers.
Each Availability Zone has independent and redundant power, networking, and connectivity.
So, the chance that two Availability Zones simultaneously fail is very, very rare.
All the Availability Zones in a region are connected through low-latency links. So, you'll not have a high performance impact when you deploy applications across multiple Availability Zones.

The biggest advantage of having multiple Availability Zones is increased availability and fault tolerance
within the same region.

Even if one of the data centers completely fails, your application will still be available if you are
deploying to multiple Availability Zones.

One of the most important things to remember is that not all Azure regions have Availability Zones.

Some of the Azure regions have no Availability Zones at all.

Some of the Azure regions have three Availability Zones.

Let's look at a few examples of Regions and Availability Zones.

East US has three Availability Zones.

West Europe has three Availability Zones as well.

Southeast Asia, Asia Pacific has three Availability Zones. Brazil South has three Availability Zones
as well.
West Central US has zero Availability Zones.

As you can see, Azure offers a number of regions around the world and some of them have Availability Zones and some of them do not have Availability Zones.

Region>Zone
