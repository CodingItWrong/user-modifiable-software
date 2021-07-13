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

There was also a marketing impact:

> At the same time Sun Microsystems’ massive marketing campaign for Java convinced enterprises that Java was the future for both web and standalone client applications. Even though Java never delivered on its client-side promises, the commercial Smalltalk vendors were unable to counter the Java hype cycle and development of new Smalltalk-based enterprise applications stopped.'

(WB)

Why wasn't there the same push from Smalltalk? I have a theory that a clue is found in something Adele Goldberg said about the founding of ParcPlace:

> Products are successful when there’s passion around the product, when you’ve done something that you’re interested in, you care about. To just say that somebody else should [support] it…I don’t think that is the message you want to give to the commercial sector. They want to know that the people who were the inventors cared about it.

(Adele)

Goldberg gave this as a positive reason for the motivation of founding ParcPlace. But on the flip side, it's telling that Alan Kay wasn't involved in ParcPlace. Kay could probably be called the main theoretical driver of Smalltalk, but he wasn't involved in developing it commercially. So there was a split focus in the Smalltalk ecosystem.

In 1997 in describing Squeak Ingalls made a point about the hope for adaptability:

> Therefore our ideal system would be a small, portable kernel of simple and uniform design that could be adapted rapidly to new delivery vehicles.

(Squeak)

However, when smartphones were introduced in 2007, Squeak was never adapted to them. Why not? My guess is that it's because smartphones are only *practically* different from desktop computers, not *theoretically* different. In the research focus that the Squeak community has, adapting Squeak to run on smartphones would not advance research of language design and computing. Unfortunately, this means that Smalltalk isn't available for development on what is now the most widespread computing platform.

As another anecdote, I share another note from Goldberg:

> There was no documentation, there were talks. And in those talks, we would say “if you want to know how to do something, you just read the code, and it pretty much self-documents”—I mean, we were so full of ourselves.

(Adele)

In trying to learn Squeak, this lack of documentation has been a barrier for me as well. There is some information in the Squeak wiki, but it's not consistently organized and edited. Once a developer finishes the _Squeak by Example_ book, generally the advice they're given is "use the Smalltalk browser." While the browser is a powerful tool for learning, it's not the same as having up-to-date and clear documentation--at least for introductory purposes.

In 2001 Ingalls wrote an optimistic take on the evolution of languages:

> Computer systems are, in fact, getting simpler and, as a result, more usable. I would like to close with a general principle which governs this process: Natural Selection: Languages and systems that are of sound design will persist, to be supplanted only by better ones.

(Design)

For anyone who believes in the benefits of Smalltalk, this principle is hard to square with the reality of Smalltalk's decline--unless the view is taken that over the long term better languages will increase.

In particular, theoretical benefits of Smalltalk's programming model aren't enough to influence businesses to adopt it:

> our customers didn’t really care about Smalltalk, or object-based programming and design, or live programming, or any of the unique technologies Smalltalk brought to the table. They just wanted to replace those green-screens with something that looked like a Windows application.

(WB)
