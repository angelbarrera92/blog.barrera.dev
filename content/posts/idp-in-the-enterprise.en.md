---
title: IDP in the enterprise
date: 2022-12-15
tags:
    - enterprise
    - culture
    - tech
cover: images/idp-in-the-enterprise.jpg
---

A few weeks ago, I spent some time understanding how an IDP could be implemented in the enterprise. I found a few articles and videos that were helpful, but I was still left with a few questions. In particular, I wanted to know **how IDP should be implemented in a siloed and political environment**. I also wanted to know how to deal with the inevitable resistance to change that would come from the different departments.

> IDP stands for **Internal Development Platform**.

<!--more-->

[Here you'll find the optimistic approach how to implement an IDP](https://github.com/angelbarrera92/idp-enterprise-research/blob/main/outcome.md), unfortunately, it assumes that the organization is well structured and that **the people are willing to change**, including the middle management, directors and, development teams.

This, unfortunately, is not the case in most organizations. The reality is that **most organizations are siloed and political**, and the people are not willing to change, even worse in economical crisis times. This is why I decided to write this article, to share my point of view after talking with a few people in the industry in the same situation.

#### The situation

It's almost *2023*, and every industry is digitalized, from retail to banks, commerces, and governs so it's a fact that **we need engineers to run a modern society.**

Most of these enterprises *succeed* in adopting the cloud. Some of them are [returning to on-prem](https://www.channelpronetwork.com/article/return-prem), but that's a topic I would like to discuss in another post.

Enterprises moved from *on-premises* to the *cloud*. Some of them tried to follow the same procedures and processes as they were following before in their data centers. That didn't work, engineers were struggling to develop and implement projects they were hiring for, resulting in managers and middle management didn't see any improvement by moving to the cloud.

At this point, they had two options:

- Keep operating as they were doing assuming the cloud is not going to provide them any higher benefit.
- Change the way of working adopting the flexibility of the cloud.

Those companies that adopted the second point, had to replace certain roles and processes in the company.
This could lead to significant changes in the company's management structure:

- Who is managing access to the cloud?
- Who is taking care of the cloud accounts?
- Can the employees use any service in the cloud?
- Who is responsible for managing the firewall on cloud instances?
- **What about the billing?**

As you can imagine, this caused a lot of difficulties for companies. These changes are *only* affecting a few IT departments which adopt automation processes and provide services to the developers.

##### Developers

Developers, *back in the day*, focus on developing business requirements. Then, they push the code somewhere else, **the job is done**.

We all agree **that's not enough**. Unfortunately, **there is no consensus about what is enough** for a developer.

- Should a developer take care of a pipeline?
- Is the developer aware of the steps the pipeline should run?
- Should the developer be aware of the security of the *pipeline/code/infrastructure/data*?

**Developers want to focus on writing code and delivering business value**, rather than worrying about infrastructure and deployment.

It's almost 2023, *in the cloud*, with *containers*, with *APIs*, with *vulnerabilities*, *contractors*, *internal development teams*, and the *CNCF*.

##### CNCF

**Cloud Native Computing Foundation**. This brought us a lot of tools and a lot of confusion. I mean, *Kubernetes*, *Prometheus*, *linkerd*, and  other projects are **amazing**. Unfortunately, every project hosted in the CNCF is a piece of software that does nothing alone. So, **you need to understand how to use them, and you need to know how to integrate them.**

This is not easy, **is this something the developer should take care of?**

The CNCF is the main reason why companies are investing today in platform teams.

#### Consequences

Onboarding is a pain in the ass, both for the employee and the employer:

- The employee has to understand a lot of different technologies and how these have been implemented in the company/project.
- Employer, trying to find a good engineer in the current market is a chimera. You would need to pay them a lot as you require from the engineer a lot of knowledge. Don't forget we are right now in an economical crisis.

Don't forget the offboarding. **Engineers want to engineer right**? So if they find better opportunities inside the same company or outside it, an engineer will pursue these opportunities, so you'll end up with unfinished projects/products.

Then, remove permissions for that particular engineer, and **try to onboard a new employee** in the project/product these days...

##### micro platforms

You'll find **micro-platforms** on different teams. *What is this?*

These are frameworks advanced developers in the team develop to **standardize the way their team works**, they are already realizing that there is a standardization problem in the company they are working on.

*What is the inevitable problem?*

They *(use to)* don't have enough context to properly implement the *(micro)* platform, and they probably could be tied to certain services the company could be giving *(ticketing system, alerting, runtime, metrics...)* and it will cause a lot of friction with the IT teams *(infra, platform, cloud, security....)*

It sounds clear to me; teams are developing their way of developing. **Then it means that there is a potential requirement in the company**, and this is standardizing the way of developing *(IDP)*.

#### The ugly truth

The main reason why there is no single internal development platform is not about tech, there are a humongous number of technologies ready to glue together to cover most of the use cases you can see in your company.

*So, what's the issue?* **Middle management**.

In a traditional enterprise, you will see a well-defined organizational structure with multiple layers of management. From the C level to the bottom you can find 3-4-5 levels of management *(even more; the larger the company is, the more levels you'll find)*.

Every manager cares about X employees and/or managers.
**The more reports the manager receives, the "more important" the manager is for the company**, at least, this is what we can see in these kinds of large companies. Also, they are used to working in a project approach, providing services for different areas. So you should expect to interact within areas through tickets/forms...

Then... What would happen if someone tries to implement an IDP that involves many different departments?

{{< image src="/images/IDPCapabilities.png" alt="IDP Capabilities" position="center" style="border-radius: 8px;" >}}

The middle management could take this *(and they do)* as an attack on their responsibilities.

#### Conclusion

I don't have a silver bullet, but I have a few ideas that could help you to start thinking about this topic.

- **Take a look at your environment**; Is your manager aware of the current situation? If not, try to explain the situation to your manager.
- **Start with the developers**. Developers are the ones who are going to use the platform, so they should be the ones who are going to define the requirements and the capabilities of the platform. **Treat them as your customers.**
- **Start small**. Start with a small team, and try to implement a micro-platform that can be used by a few teams. Then, try to expand the platform to other teams by presenting the benefits of using this platform to your manager.
- **Start with the basics**. Start with the basics, and try to implement a platform that can be used by all teams in the company.

You should be together with your manager to present the benefits of using the platform to the other managers.
You should be able to show them how the platform can help them to improve their processes and how it can help them to improve the way they are working.

**Implemented successfully, it will save a ton of money for the company**
