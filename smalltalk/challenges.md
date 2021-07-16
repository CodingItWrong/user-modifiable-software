---
title: 'Smalltalk > Challenges'
---

What caused Smalltalk's decline? Smalltalk has always been a controversial platform so there are surely different views. This page doesn't attempt to survey all viewpoints, but only to record the credible information I've found so far.

Allen Wirfs-Brock records that Smalltalk's industry adoption rapidly declined:

> Over six months in 1996, Smalltalk’s place in the market changed from the enterprise darling COBOL replacement to yet another disappointing tool with a long tail of deployed applications that needed to be maintained.

(WB)

What was the cause of this decline?

Slow performance is a regular criticism of dynamic languages by statically-typed language advocates, and while this was true in early Smalltalk, Wirfs-Brock asserts that that was not a problem at the time of Smalltalk's decline.

The way source control is handled in Smalltalk is also different than source-file-based languages, because classes exist as objects in the image memory. But Wirfs-Brock also asserts that source control was handled.

The biggest cause of the decline, according to Wirfs-Brock, was the web:

> The World Wide Web diverted enterprise attention away from fat clients and suddenly web thin clients were the hot new technology.

(WB)

Java capitalized on this with a marketing campaign:

> At the same time Sun Microsystems’ massive marketing campaign for Java convinced enterprises that Java was the future for both web and standalone client applications. Even though Java never delivered on its client-side promises, the commercial Smalltalk vendors were unable to counter the Java hype cycle and development of new Smalltalk-based enterprise applications stopped.

(WB)

Why wasn't there the same marketing push from Smalltalk? I think a clue is found in something Adele Goldberg said about the founding of ParcPlace:

> Products are successful when there’s passion around the product, when you’ve done something that you’re interested in, you care about. To just say that somebody else should [support] it…I don’t think that is the message you want to give to the commercial sector. They want to know that the people who were the inventors cared about it.

(Goldberg 58:12)

ParcPlace was founded by some of the creators of Smalltalk and this did demonstrate to the commercial sector that some of the inventors cared about it. But, tellingly, Alan Kay was missing. He didn't have an interest in developing Smalltalk commercially. And I think this split focus was apparent to the commercial sector.

In 1997 Ingalls expressed a hope that Squeak would be a highly adaptible Smalltalk:

> Therefore our ideal system would be a small, portable kernel of simple and uniform design that could be adapted rapidly to new delivery vehicles.

(Squeak)

However, when smartphones were introduced in 2007, Squeak was never adapted to them. Why not? My guess is that it's because smartphones are only *practically* different from desktop computers, not *theoretically* different. In the research focus that the Squeak community has, adapting Squeak to run on smartphones would not advance research of language design and computing. Unfortunately, this means that Smalltalk isn't available for development on what is now the most widespread computing platform.

I think another challenge to Smalltalk's adoption today is a lack of documentation. Goldberg saw this problem looking back:

> There was no documentation: there were talks. And in those talks, we would say “if you want to know how to do something, you just read the code, and it pretty much self-documents”—I mean, we were so full of ourselves.

(Goldberg 41:44)

In trying to learn Squeak, this lack of documentation has been a barrier for me. There is some information in the Squeak wiki, but it's not consistently organized and edited. Once a developer finishes the [*Squeak by Example*](https://wiki.squeak.org/squeak/6546) book, generally the advice they're given is "use the Smalltalk browser"--a tool that allows exploring class and method definitions live. While the browser is a powerful tool for learning, it's not the same as having up-to-date and clear documentation--at least for introductory purposes.

In 2001 Ingalls wrote an optimistic take on the evolution of languages:

> Computer systems are, in fact, getting simpler and, as a result, more usable. I would like to close with a general principle which governs this process: Natural Selection: Languages and systems that are of sound design will persist, to be supplanted only by better ones.

(Design)

For anyone who believes that Smalltalk has a sound design, this idealistic principle is hard to square with the reality of Smalltalk's decline. In particular, whatever the theoretical benefits of Smalltalk's "sound design," those in themselves aren't enough to influence businesses to adopt it:

> …our customers didn’t really care about Smalltalk, or object-based programming and design, or live programming, or any of the unique technologies Smalltalk brought to the table. They just wanted to replace those green-screens with something that looked like a Windows application.

(WB)
