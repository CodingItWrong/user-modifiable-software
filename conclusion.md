---
title: 'Conclusion'
---

How do Smalltalk and HyperCard empower people?

Smalltalk attempts to empower people by creating an environment that makes it easier to learn to program. When using software, you can inspect it to see what objects are behind it. To make adjustments to it or to create your own software, you will need to begin programming. Once you do, there is no limit to what you can customize, because almost everything in the Smalltalk environment is written in itself.

HyperCard attempts to empower people by maximizing your ability to create interactive software with no or minimal programming. You can first create by inspecting and modifying stacks in a graphical interface, including things like linking buttons to other cards. Then you can go further by finding buttons in stacks or libraries and copying them into your stack along with their behavior. From there you can begin scripting using the accessible HyperTalk language. At that point, though, the learning curve spikes. To extend the environment to do something that isn't built in you need to get different programming tools and program in a different language. And you can't change HyperCard itself: it's proprietary compiled software.

The effect was that HyperCard provided a smoother on-ramp to begin creating software, because you didn't need to start out programming at all. But HyperCard had a hard limit on how much you could accomplish, meaning that Smalltalk was better suited for research and ongoing evolution.

HyperCard created a dynamic environment by imposing constraints: a limited set of primitives you can graphically lay out and program. As a result, it created a hobbyist programming segment. Smalltalk created a dynamic environment with very few constraints, by building up from a low level with a dynamic setup. This allowed rapid innovation leading to today's graphical computing paradigms. In the middle is traditional compiled development. It has the same lack of constraints as Smalltalk but is much higher effort to develop in, making it hard to broadly innovate. Instead, traditional development advances by individual systems, like the web, SQL, and mobile operating systems. These paradigm shifts undercut Smalltalk by being able to be developed in a performant way, and are composable to build on top of. In other words, when you *do* get a good technology traditionally, it's much more easy to build on it.

The result is a spectrum where on one end is hobby development which is best suited to dynamic environments, in the middle is commercial development which is best suited to compilation, and at the other end is research which is best suited to dynamic environments.

***

The things that traditional software don't support that HyperCard and Smalltalk do: is there a need for them? Do many users need to customize their software? Do many users need to create interactive experiences?

It would be easy to look at market pressures and say that the answer is no. Commercial and traditional source-code-based open-source software is sufficient for most users most of the time, including the customization settings they offer. And the benefits of those environments for providing full-featured functionality outweigh any slight benefits that customization might provide. And people don't want or need to create interactive experiences: they want to create documents and post to social media.

I think there are a few reasons not to take this view. First of all, the fact that people make do with limitations in software doesn't mean it's ideal. People adapt to what they're presented with, even to the extent of handling things that are significantly harmful to them. Instead of forcing users to adapt to software, it would be ideal if people could adapt their software to themselves.

As an example of adapting software to yourself, I recently switched from using Twitter to Mastodon, an open-source social network. I found a certain feature, the "federated timeline", that I usually regretted looking at due to content I objected to, but I found myself continually tempted to check it to pass the time. I couldn't find a client app that provided a setting for me to hide the federated timeline. So I forked an open-source iOS client app and made a one-line change to remove the button to show the federated timeline. This has resulted in a much better experience for my mental health. Instead of needing to exert the effort to resist the temptation to tap that button, or endure the consequences of looking at content I didn't want to, I was able to adapt my software to meet my needs. Now, I was only able to jump through the hoops to accomplish this this because I've done iPhone development in the past; non-developers don't have this option.

Second, Henry Ford and Steve Jobs famously designed products based not on what people were asking for but based on a vision for what they would really benefit from. Now, I'm no visionary like Ford or Jobs, but I don't have to be: all I have to do is look at the impact Smalltalk and HyperCard have had in the past.

Bill Atkinson said:

> I'm a populist. I want everybody to be empowered. I think the more people that are empowered, and particularly those that have passion about something, and they want to share it with other people--

(Legacy 15:00)

If the question you ask is "do users who are not developers need the ability to create or modify software," you've biased the question: you've assumed a distinction between users and developers. Instead of making that assumption, what if we just thought about people? Then the question might be "does it benefit people to empower them to create software more easily?" And I think the obvious answer is yes. We should find ways to allow developers to create software more complex than they ever have before. We should make it easier for developers to create software of the same complexity we've created before, by creating good abstractions and elimitating accidental complexity. We should make it easier for people to learn to become developers. And we should make it easier for people to create and modify software without having to become a developer.

One of the powerful things about HyperCard and Smalltalk is that there are no technical barriers between users and developers. There is no need to install and set up a complex separate environment, and configure complex build tools. In HyperCard, you're a user, and you're at a certain user level. Some users are at typing level, and others are at authoring, others scripting. And even if you're programming to create a custom function or command, that's all in service of being a HyperCard user. In Smalltalk, your software runs in the same environment you program it in.

***

If we argue that it would be beneficial for users to have the ability to modify their software, then what would it take to create a modern platform to do so? It would need to have the following attributes:

- It would need to run on both desktop and mobile devices, even accounting for Apple's App Store restrictions.
- It would not need to support every hardware and user interface feature of the platforms it runs on, but it would need to provide enough of a toolkit to create useful software, including operating on different form factors.
- Users would need to have a way to easily share the software they create with one another.
- When a user is using the software, they would need to already have all the tools they need to inspect it and modify it.
- There would need to be a way to make ongoing development and maintenance economical, even though it would not be possible to charge for the platform so that it can function as an exchange medium. Presumably, it would need to be open source.

None of these needs are technically insurmountable. There is some creativity required around figuring out what toolkit of functionality is useful and what mechanism of sharing works best. The main challenge is economic: can something be created that is useful enough to bootstrap enough interest to get community support to continue open source development? It remains to be seen.

***

Alan Kay, one of the creators of Smalltalk, famously takes a long-term view on computing. In "The Computer Revolution Hasn't Happened Yet" he describes what it would take for computing to reach its destiny, allowing computational complexity to scale by factors of a trillion, to match the computational complexity that already happens in living organisms. I don't have the foresight to assess that view or make my own prediction for what the far future of computing should be. But I can do what Bill Atkinson suggested and "make ethical and aesthetic choices about different futures."

In my assessment, it is better for software to empower people more instead of less. Because of this, it is worthwhile to invest in finding new ways to empower people to create and modify their software. A given avenue of research may fizzle, or may prompt the next idea that has more of an impact, or it may itself have an impact for a few people or many, for a year or twenty. But trying to find ways to empower people with software is a goal that is worth the effort.
