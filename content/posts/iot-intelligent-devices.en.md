---
title: IOT - Intelligent Devices
date: 2022-12-02
tags:
    - IOT
    - lay
    - future
    - tech
cover: images/iot-intelligent-devices.jpg
---

I recently discovered that my vacuum robot stopped working for more than three days.

I could not configure the vacuuming program, that is, I could not modify the cleaning plan to define the rooms to be cleaned nor modify the suction power that the application allows you to set **and you cannot do it in any other way**.

<!--more-->

#### Then?

Actually, you can turn the robot on with the button on the device itself and it will perform the last run it was configured to do. Hopefully it will be the entire house at sufficient suction power.

After a few days, the app started working again... but this gave me pause. We rely on third-party services when we buy certain products, such as robot vacuums, smart plugs, surveillance cameras, etc.

In this situation there are *(mainly)* two groups of people:

- **Common people** who do not have to know these details and buy this kind of devices because they like or need them.
  They think they can be a good solution for them, but in this kind of situations, the only thing they can do is to call the store where they bought it or call the manufacturer to manage the warranty.
- **Computer scientists** or those of us who like to solve technological problems and understand how this type of devices work, i.e. we know that they connect to a remote server to send/receive data *(which we don't usually like)* and that we need to interact with them from inside and outside the home through an application.

#### Surveillance cameras

These also apply to surveillance cameras. The common use of a surveillance camera is to be able to see what is happening in the house in real time from anywhere. In addition, upon any event/movement to receive security notifications. For this we rely, implicitly, on external services.

Are users aware of how this works? If they knew that the images pass through a server of a company *(which may or may not be the manufacturer of the product)*, the content is analyzed and stored in the cloud, would they buy it? Would they use it? Would they install it at home?

The general public does not have to know this detail, for most it is just an application which configures the surveillance camera and magically you can see what happens in your home from anywhere in the world.

But **magic does not exist**, on this we all agree.

#### Alternatives

I found a group of affected *(on telegram)* and it turns out I wasn't the only one.... The reason was that the servers of this brand went down and was out of service during that weekend completely.
In this telegram group I discovered that there was a way by which to set up a compatible server on my own. This way, I would be the only one responsible for keeping the service running so I could use my robot vacuum cleaner and be able to configure it without having to depend on that third party company.

After several hours of reading information and after studying *(not trivial)* how to access and re-configure *(root)* the robot to use this new method, I finally got it working.
All this is only feasible if you are a computer scientist and like this kind of stuff.

#### Future

For the general public I foresee legal problems with warranties, ie:
- What if your robot vacuum cleaner stops working?
- What if it stops giving you certain functionality if a company's server stops working?
- What if the company goes bankrupt?
- o... any other reason that makes you unable to use that application to configure your device?

*Is there some kind of law that mandates that you have to support and provide services for at least the life of the device?*

If not...

*What responsibility does the company have to maintain the server or that service beyond a year or two years from the sale of the product?*

I mean, we could get to a point where your device is a paperweight, right? **Even if it's in good shape**.
There may come a time when you can't use your device at all because the company has stopped providing services and it all goes straight to the junkyard.

I foresee the following situations:

- Legislate to avoid these situations. It has loopholes:
  - How can you force a company outside the EU to provide service for the lifetime of a device?
- Return to non-intelligent devices.
  - Consumers will prefer to spend more money and have their device work regardless of whether the company goes bankrupt so they can fully enjoy their device.
- Companies dedicated to servicing these devices.
  - *Not usually economically viable/profitable*.
