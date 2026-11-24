---
title: "Interlude: Why I Created the Quake Bot Archive"
weight: 11
---

# Interlude: Why I Created the Quake Bot Archive

I didn't set out to become a Quake archivist.

I certainly didn't plan to spend hundreds of hours tracking down old ZIP files, searching through forgotten websites, and reconstructing the release histories of Quake modifications that were nearly thirty years old.

It started because I wanted to play some Quake.

During the COVID-19 pandemic, like a lot of people, I found myself returning to games I had enjoyed when I was younger. For me, that meant Quake.

I started playing through all the popular single-player maps and episodes I could find. There were hundreds of them, ranging from small experimental maps created in the 1990s to enormous, beautifully designed episodes released decades after the original game.

I was having a wonderful time.

I started recording my playthroughs and uploading them to YouTube, partly to share the experience and partly to keep a record of everything I had played.

You can still find those videos on my old YouTube channel:

* [Quake Buffet](https://www.youtube.com/@quakebuffet)\
	`https://www.youtube.com/@quakebuffet`

This continued for several years. I played hundreds of maps and episodes, rediscovered old favourites, and gained an even greater appreciation for the creativity and dedication of the Quake community.

Eventually, I started thinking about something else I remembered fondly from the early days of Quake.

Bots.

## Rediscovering Quake Bots

If you played Quake in the late 1990s, you might remember the excitement surrounding the first computer-controlled opponents.

Today, playing against bots is an ordinary feature of multiplayer games. But back then, the idea that someone could write a modification that introduced intelligent opponents into Quake was extraordinary.

I remembered the classics, particularly the Reaper Bot. I also remembered more sophisticated bots such as the Omicron Bot, and later projects such as FrikBot and Frogbot.

I thought it would be fun to download some of these old bots and play against them again.

How hard could that be?

I started searching the web and quickly found some old mirrors containing Quake modifications.

One particularly useful resource was the [Quaddicted mirror of the old idgames2 bot directory](https://www.quaddicted.com/files/idgames2/quakec/bots/) (`https://www.quaddicted.com/files/idgames2/quakec/bots/`).

This was a surviving mirror of the original `/idgames2/quakec/bots/` directory from `ftp.cdrom.com`, one of the most important distribution sites for Quake modifications in the 1990s.

It was a wonderful discovery.

There was the Reaper Bot, the BGBot, along with many other early bots I remembered or had heard about. I downloaded them, started Quake, and had a great time experimenting with these old creations.

But something was wrong.

The directory contained plenty of early bots, but many of the later, more sophisticated bots from 1997 through 1999 were missing.

Where were they? Wasn't this directory an archive of all quake bots? I guess not...

And what about the bots that were there but didn't work?

I remember coming across the OakBot from the `/idgames2/quakec/bots` directory and struggling to get it running. Surely there had been updated releases. Perhaps an earlier version would work better. Where were those files?

I searched around, but there was no obvious answer.

## Where Were All the Files?

The more I looked, the more questions I had.

Take FrikBot, for example.

I could find a copy of FrikBot, but how did I know it was the latest version?

What was the final release? Were there patches? Had development continued after the version I'd found?

It turned out that FrikBot had received numerous updates during the early 2000s.

Where were all those releases?

Or consider the Omicron Bot, often called the obot.

This was one of the great Quake bots, created by Jan Paul van Waveren, better known in the community as *Mr. Elusive*.

He later went on to work at id Software and developed the bot AI for Quake III Arena, a remarkable piece of engineering in its own right.

The Omicron Bot was an important step along that journey.

I wanted to revisit it, understand how it worked, and perhaps study its implementation.

But where was the source code?

Had it ever been released?

If not, perhaps an earlier version of the modification included it. Perhaps a development release had survived somewhere. Perhaps there were old discussions explaining how the bot worked.

I had no idea.

And there didn't seem to be anywhere I could go to find out.

I could find individual downloads, scattered references, old websites, and fragments of release histories. But I couldn't find a comprehensive archive of Quake bots that brought everything together.

I wanted to see all the known bots, all their releases, their source code where available, and something of the history behind their development.

Surely someone had already done this?

Apparently not.

## Why This Bothered Me So Much

This probably sounds like a rather obscure problem to become obsessed with.

After all, I was trying to play computer-controlled opponents in a game from 1996. Did it really matter whether I had the final version of a particular bot, or whether an earlier release included source code?

To me, it did.

Quake bots were a big deal.

In the late 1990s, there were entire communities devoted to developing them, testing them, and discussing how they worked.

People experimented with navigation, pathfinding, combat behaviour, decision-making, and all sorts of techniques for creating believable opponents.

These weren't just game modifications. They were experiments in artificial intelligence.

And for me, they were much more than that.

**Quake bots were one of the things that first got me interested in programming and artificial intelligence.**

The idea that you could write code to create an opponent that moved around a three-dimensional world, made decisions, and reacted to a human player was fascinating. It is still fascinating!

That fascination helped set me on the path toward studying computer science and eventually completing a PhD in artificial intelligence.

So when I returned to these old bots decades later, I wasn't just revisiting a game.

I was revisiting something that had helped shape my interests and, ultimately, my career.

I knew how much creativity, experimentation, and technical effort had gone into these projects. I knew that people had spent countless hours developing them, sharing their ideas, and building communities around them.

Yet much of that work seemed to be disappearing.

The original websites were gone. Download links were dead. Release histories were incomplete. Source code was difficult to find, when it could be found at all.

It bothered me that these projects, which had once seemed so important, were slowly fading from the internet.

And it bothered me even more that there was no single place where someone could go to explore their history.

I wanted that archive to exist.

## A Wrong in the Universe

Eventually, I reached a simple conclusion.

If nobody had created a comprehensive archive of Quake bots, perhaps I should create one myself.

It felt like a small wrong in the universe that I might be able to put right.

I wasn't particularly interested in creating another download directory containing a handful of ZIP files.

I wanted to know what had actually been released.

I wanted to find the original distributions, track down different versions, establish release dates, locate source code, identify the developers, and reconstruct the history of these projects as accurately as I could.

I wanted someone interested in a particular bot to be able to find not just a download, but the story of that bot's development.

And so I started building what became the:

* [Quake Bot Archive](https://github.com/Jason2Brownlee/QuakeBotArchive)\
	`https://github.com/Jason2Brownlee/QuakeBotArchive`

![The Quake Bot Archive, documenting the history and releases of Quake 1 bots.](/QuakeBotArchive.png)\
_Figure: The Quake Bot Archive, documenting the history and releases of Quake 1 bots._

At first, I thought it would be a relatively small project.

Find the bots. Collect the releases. Write down what I knew. Put everything somewhere public.

Of course, it wasn't that simple.

Every bot raised new questions.

A missing version would lead to an old website. That website would mention another release. The release announcement would point to a long-dead FTP server. Somewhere in an archived forum discussion, someone would mention a patch or an experimental build that I had never heard of.

I would find one file and discover references to three more.

Sometimes I spent hours looking for a particular release and found nothing.

Other times, an obscure mirrored FTP directory would turn up exactly what I had been searching for.

And occasionally I would stumble upon something I hadn't even known existed.

It was frustrating, fascinating, and enormously rewarding.

I was hooked.

## One Archive Leads to Another

I spent hundreds of hours researching, collecting, organising, and documenting old Quake bots.

Along the way, I discovered that preserving the files was only part of the challenge.

To understand when a particular bot was developed, what features it supported, or which version of Quake it was intended to work with, I needed a better understanding of the history of Quake itself.

When had the different official versions of Quake been released?

When had the QuakeC source code been updated?

Which engine changes might have affected a particular modification?

I found myself repeatedly looking up the same information.

So I did what was beginning to feel like the obvious thing.

I created another archive.

This time, I focused on the official releases of Quake, documenting the different versions, updates, and source code releases.

It gave me a reliable historical reference that I could use when researching modifications.

And, naturally, that project raised more questions and suggested more things worth preserving.

One archive led to another.

Before long, what had started as a simple desire to replay some old Quake bots had turned into an ongoing hobby of researching and preserving Quake history.

I've spent years creating new archives, revisiting old ones, filling gaps, correcting mistakes, and following leads wherever they took me.

One of the unexpected pleasures was making contact with people in the Quake community.

I discovered that, nearly thirty years after the game was released, there were still people who cared deeply about these old projects.

Some had been involved in the original modding scene. Others were newer enthusiasts who had discovered Quake long after its heyday.

People shared files, answered questions, offered corrections, pointed me toward forgotten resources, and told stories about projects they had worked on decades earlier.

These conversations became some of the most rewarding parts of the entire experience.

What began as a solitary search through old files turned into a way of connecting with people who shared an enthusiasm for preserving this small corner of gaming history.

## You Only Need a Reason to Start

Looking back, I never would have guessed where that first search for the Reaper Bot would lead.

I just wanted to play some old bots.

Then I wanted to know whether I had the latest versions.

Then I wanted to find the missing releases.

Then I wanted to understand their history.

And eventually, I wanted to make sure that someone else, perhaps years or decades from now, wouldn't have to repeat all the searching I had done.

That's how the Quake Bot Archive began.

I share this story because I think it illustrates something important about preservation.

You don't need to begin with a grand plan to preserve gaming history.

You don't need to be an expert archivist. You don't need special tools, an enormous collection of files, or the backing of an organisation.

You just need something you care about.

Perhaps it's a modification you played as a teenager. Perhaps it's a forgotten map pack, an obscure multiplayer mod, or a tool that you remember using years ago.

Perhaps you simply want to know what happened to a project you once loved.

Start looking.

Ask questions. Follow the leads. Keep a record of what you find.

And if you discover that nobody has brought all that information together, perhaps you're the person who should do it.

That's what happened to me.

I went looking for some old Quake bots and ended up becoming their archivist.

**Sometimes, that's all it takes.**
