# Timothy Southwick's Portfolio

## About Me

I am a software engineer with a Masters in Computer Engineering from UMass Lowell and a focus in digital processor design. My hobbies include robotics and software development. I've used Linux as my primary operating system since 2009.

My interest in software started in elementary school when I took up a hobby of writing and testing software using Lego Mindstorms robotics. By high school, I was able to program my graphing calculator to automate the process of solving tedious math and science problems. I asked my teachers if I could use those programs, explaining that I would need to understand the formulae involved in order to program them. To my teachers' surprise, I was successful in writing each program and was allowed to use them in class.

In college I discovered a Minecraft server network called Monumenta, which is unusual in that it has a weekly update cycle that merges newly developed terrain with existing player inventories. At the time, these weekly updates were manual and error-prone, causing delays. I was excited to rise to the challenge and automate this process to make the developers' lives easier and get players back into the game sooner. After submitting changes for a few days to meet the specification, I was added to the team and my code was used in production. Within a year (April 2018) I was promoted to team lead for my technical contributions. I have been an active lead developer ever since.

## [Monumenta](http://www.playmonumenta.com/)

I am a lead developer and co-owner for Monumenta Games LLC, under the username NickNackGus. I mostly work on the tools and infrastructure that make the game possible, with a few small player-facing features on the side. Some of my most recent and advanced work can be found in [our repositories](https://github.com/TeamMonumenta).

### [Network Chat](https://github.com/TeamMonumenta/monumenta-network-chat/)

Overview:
- Allows chat between multiple Minecraft servers
- Features multiple chat channels
- Settings and permissions to control access and visibility
- Users may set any channel as their default chat, including direct messages
- Chat may be paused for text-centered user interfaces

Technical aspects:
- Configuration saved to Redis, cached by each server
- Inter-server communication via RabbitMQ
- Chat messages are transmitted as JSON for easy logging and external chat integration

### [Automation](https://github.com/TeamMonumenta/monumenta-automation)

Technical aspects:
- JSON-like parser for Mojangson data format used by Minecraft's command system
- Recursive data structure iterator to find inventory items nested in various item containers, which may themselves be items
- Contains configuration for Kubernetes deployments

### [Scripted Quests](https://github.com/TeamMonumenta/scripted-quests)

A json-based quest system for Minecraft that I helped develop

#### [Zones](https://github.com/TeamMonumenta/scripted-quests/pull/58)

This system allows us to tag regions of space with text-based properties. For example, marking a town as "no building", and "no hostile mobs". It was written with runtime speed in mind, identifying the appropriate properties for a given location in O(log(n)) time. For best runtime results, startup and reload times were sacrificed. Reloading zones was made asynchronous to accommodate this without affecting in-game performance.

## Contact Info

Email: Timothy.Southwick94@gmail.com

Phone: 978-857-7943

LinkedIn: https://www.linkedin.com/in/timothy-southwick
