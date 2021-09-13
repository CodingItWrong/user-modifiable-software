---
title: 'An Interview With Ted Kaehler'
---

The following is an interview conducted via email with Ted Kaehler, who was in the unique position to have worked extensively both on Smalltalk and HyperCard. Ted, thank you for sharing this valuable history. The interview was conducted September 2021.

Ted's experience:

- Worked on Smalltalk 72, 74, 76, 78, and 80 at Xerox PARC.
- Worked on HyperCard and Squeak at Apple.
- Worked on Squeak and Etoys at Disney Imagineering.
- Continued work on Squeak at ViewPoints Research, Hewlett-Packard Research, SAP, and Y-Combinator's HARC.

***

**1. Did you and the other creators of Smalltalk have a conscious goal
to empower users to inspect and modify their software? If so, what
motivated that goal?**

Yes, absolutely.  Alan Kay wanted to build a "personal computer
for all ages."  Just as writing and music are each a kind of
"literacy", so the ability to build simulations and play with them
would be a new literacy.  Simulations help a student understand
anything that changes over time.  The spread of an epidemic or the
growth of a forest fire are great examples.  Every child should
become empowered to do simulations.

We admired the LOGO project at MIT.

Smalltalk-72 was very much a kids language, and we regularly
brought kids up to our lab at Xerox PARC.


**2. Were there any changes to Smalltalk over time that affected how
easily users could inspect and modify code?**

We were devoted to letting users "see" their code better and
more simply.  Larry Tesler created the "Code Browser" to let users
see the classes and methods of the entire system.  Dan Ingalls
implemented the first opaque overlapping windows to let users see
more code and other objects on the screen.  Dan invented pop-up menus
to put editing commands where the user was working at that moment.
We made searching for all senders of a method and for all
implementors of a method very easy in Smalltalk.  Dan implemented
name completion for method names for when a user can't think of the
whole name.  Scott Wallace's "Selector Browser" lets a user search
for a method using a fragment of its name.  My "Method Finder" lets a
user find a method by giving an example of its input and output.
(Type 'joining '.  'two strings'. 'joining two strings'.  in the
Method Finder.  It searches and discovers "," as the message that
concatenates.)

We experimented with showing code in a "Galley" instead of
one method at a time.  We avoided putting code in files so the user
would not have to think about or manage files.

Everything in Smalltalk is an object, and the only thing you
can do is to send a message to an object.  That idea clarifies user's
thinking about how to write a program.  Classes of objects and the
messages they can receive are a great way to logically organize code.
Each class has an external interface.  The user is free to change the
internals of a class.  The entire rest of the system is guaranteed to
work if the interface of the class stays the same.  This is a very
common idea now, but it was new and radical in 1974.

Dan and Alan made each class be an object on equal footing
with other objects.  While LISP had all parts of the system
accessible to programmers, having classes as objects made this much
clearer and easier.  Code written by users is treated the same as
code that came with the system.

There is a famous email from a user about the greatness of
the "24-hour Smalltalk Support Desk."  There is no such thing of
course, but this user realized that everything about the system is
visible and changable.  At 3 am he realized he needed to change the
process scheduler.  He read enough code to find the right method,
changed it, and continued with his project.


**3. What got you interested in working on HyperCard?**

As hard disks became available, I got interested in information
and how to find it.  I did a project on this at Xerox PARC.  When I
moved to Apple in March 1985, Bill Atkinson was showing a mockup of
HyperCard.  This was exactly what I was looking for.  It had fast
seach.  It had links between cards.  I helped Bill turn the mockup
into a real app.  Development was partly driven by the requirements
of the HyperCard Help Stack, which my wife Carol Kaehler was making.
She needed an unchanging background for a group of cards.  She needed
multiple backgrounds in a stack.  She needed scripting to make
buttons navigate between cards.  She needed scripts to show what each
paint tool could do.

Dan Winkler did a superb job creating the scripting language.

HyperCard came very close to being the World Wide Web six years
before the web.  Stacks could be on servers and users could browse
them.  A stack could be a mini-application on a server.  We just
didn't push it hard enough.  Connections were only over AppleTalk and
not the Internet.  It wasn't legal for a company to be on the
Internet in 1987-88.

We believed in users being able to modify a stack, and were
opposed to the locking that a page on a server needs.  (Though,
HyperCard does support the correct kind of locking.)


**4. When you began working on HyperCard, did you see it as a
continuation of some of the themes of Smalltalk's development
experience, or as something very different?**

HyperCard evolved a lot during its development and Alan Kay was
advising Bill Atkinson.  Bill had very clear goals for HyperCard, but
Alan and I did try to push it in certain directions.  HyperCard was
aimed at end users, and for us it was like a second try at putting
programming in their hands.  HyperTalk scripts were command-based.
We pushed for letting scripts send messages to objects.  The objects
were cards, text fields, buttons, backgrounds, and stacks.  Bill
improved that by making dozens of built-in messages from events, such
as mouseDown.

Backgrounds are somewhat like classes in Smalltalk.  A change
there effects many cards.  Alan and I argued for generalized objects
and classes, but Bill wanted to keep it very concrete.  He was right.
A much wider group of end users were able to handle the objects in
HyperCard.  When users needed objects that were not cards or buttons,
they made cards that they never showed to the user.

We knew that Smalltalk was weak as a vessel for holding and
showing a lot of text and images.  It was not very easy for end users
to create cards and fields in Smalltalk.  HyperCard did that so well.
It was one direction we wanted Smalltalk to go, and HyperCard took it
very far.

Scripting in HyperCard is very accessible, and that certainly
furthered a goal we had for Smalltalk.

**5. HyperCard has the concept of user levels, whereas Smalltalk does
not. What difference did that make in how the two systems empower
users?**

User levels are good, especially when a teacher wants his
students to have a certian experience, and to not look at the answers
under the hood.  But, in the end, we very strongly want every user to
be on the author level.

Later, we built an end user system in Smalltak called Etoys.
It has three user levels.  The author creates an experience for her
users.  Etoys is easy to use but highly constrained.  When the author
needs more power, she can escape to the full power of Smalltalk that
is underneath.

**6. What were some of the things people have created with Smalltalk
and HyperCard that impressed you the most at the time?**

Apple estimated that HyperCard had six million author-users,
many of them teachers.  Almost every teacher had an idea for an app
for their students, and HyperCard let them create that app.  Carol
Kaehler had a role collecting and reviewing stacks from universities
after HyperCard came out.  The stacks were impressive.

Macintosh User Groups and stack exchange groups played a huge
role in popularizing HyperCard.  Apple employee Bill Fernendez helped
these groups in many ways.

One of the best features of HyperCard was the easy user
interface for card design and layout.  It was so easy for a user to
place buttons and fields and digital paint images on cards.  When it
looked really good, and there was a card for every part of the app, a
user said to herself, "I'm almost done!  All I have to do is make
these buttons work."  That, of course, was the hard part, but the
author was so jazzed by seeing her app right there, that she plunged
in and made it work.

Impressive Smalltalk programs were Alan Borning's ThingLab, a
graphical constraint system.  Adele Goldberg's job shop simulation
that we showed to the Xerox executives was impressive.  So was Steve
Weyer's Library card catalog and checkout system in ST-74.

Each version of Smalltalk was created as a simulation in an
earlier version Smalltalk.  It was particularly easy to make a new
functioning class heirarchy along side the existing one.
Smalltalk-76 was quite a bit different from ST-74, and it was vital
to build one inside of ST-74.  New data formats for objects were easy
to simulate.  Dan Ingalls got as far as running a simulated version
of the compiler for ST-76 to verify that it would work once we
"crossed the bridge" to the new system.


**7. Do you think users today would benefit from more ability to
inspect and customize their software?**

Absolutely!  It is sad that we have lost this capability in so many apps.


**8. Today, where do you see people working on ways to empower users to
inspect and modify their software?**

&lt;&lt;&lt; I'll let others answer this question &gt;&gt;&gt;
