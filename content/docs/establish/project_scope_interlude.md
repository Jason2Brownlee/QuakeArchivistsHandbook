---
title: "Interlude: A Lesson in Scope Creep"
weight: 11
---

# Interlude: A Lesson in Scope Creep

When I started the Quake Bot Archive, I thought I had chosen a reasonably well-defined topic.

I wanted to preserve all the bots created for Quake.

Simple enough.

- [Quake Bot Archive](https://github.com/Jason2Brownlee/QuakeBotArchive)\
	`https://github.com/Jason2Brownlee/QuakeBotArchive`

A bot, in this context, was a modification that added a computer-controlled opponent to the game. These opponents were primarily designed for deathmatch, allowing players to enjoy multiplayer-style combat without needing other human players.

There were plenty of these modifications, but the number seemed manageable.

I started collecting the different bots, identifying their developers, tracking down their releases, and reconstructing their histories.

I even drew a mind map showing how the different bots were related.

Some were entirely independent projects. Others were derived from earlier bots, borrowed ideas from one another, or shared portions of their code.

It was fascinating to see how these projects had evolved and influenced one another.

I felt I had a clear topic, a natural boundary around what belonged in the archive, and a collection of projects that could reasonably be researched and documented.

Then I started making exceptions.

## Just One More Type of Bot

The first expansion seemed harmless.

My original focus was on deathmatch bots, but I started finding modifications that added computer-controlled opponents to single-player Quake.

These weren't necessarily deathmatch opponents. Some were enemies or characters that behaved more like players, using weapons, navigating levels, and interacting with the environment. Helper bots, dog bots, victim bots, and more.

They were interesting examples of Quake bot technology, and I thought they deserved to be preserved alongside the deathmatch bots.

So I expanded the archive to include single-player bots.

I did draw a line, however.

Some modifications included very simple decoys or stationary figures that resembled players but had little or no artificial intelligence.

I decided these didn't qualify.

That seemed like a sensible distinction. I was interested in modifications that attempted to create autonomous opponents, not simply objects that looked like players.

The scope had expanded, but it still felt manageable.

Then I started looking at modifications that included bots.

## When a Bot Is Only Part of a Mod

Some Quake bots were designed specifically to be incorporated into other modifications.

FrikBot is a good example.

Rather than being limited to a single standalone modification, FrikBot was designed so that other developers could integrate bot functionality into their own projects.

This was an important part of its history.

If I wanted to document how FrikBot evolved and how it was used, wouldn't it make sense to preserve some of the modifications that incorporated it?

And what about modifications that included their own custom bots?

Some developers created entirely new bot implementations for their projects. Others started with an existing bot and modified it extensively to support their particular game mode.

These were interesting developments in Quake bot technology.

I wanted the archive to reflect them.

So I started including modifications that contained bots, even when the bot wasn't the main purpose of the modification.

At the time, this seemed like a reasonable decision.

Looking back, I think it was probably a mistake.

The problem is that there are an enormous number of Quake modifications that happen to include a bot.

Once you start including any modification with bot functionality, the boundary of the archive becomes very difficult to define.

Should I include a large multiplayer modification simply because it has a bot?

What if the bot is a minor feature?

What if the modification uses an existing bot with only a few changes?

What if a later release adds bot support, but earlier releases do not?

Should I now preserve the entire release history of that modification, even though most of it has nothing to do with bots?

Each decision leads to another question.

And each additional modification brings its own release history, missing files, developer websites, documentation, and research problems.

Suddenly, I wasn't just preserving Quake bots.

I was preserving a potentially enormous collection of Quake modifications that had some connection to bots.

The scope had become much broader than I originally intended.

## Another Kind of Bot Entirely

Later, I encountered another interesting category: client-side bots.

Most traditional Quake bots are server-side modifications. They run as part of the game logic and create computer-controlled opponents within the game.

Client-side bots work differently.

They are external programs that connect to a Quake server over the network, appearing to the server as ordinary players.

Instead of modifying the server's game logic, these programs act as automated network clients.

From a technical perspective, this is a fascinating approach.

It involves different challenges, different implementations, and a different history from traditional QuakeC bots.

Naturally, I wanted to preserve these programs too.

After all, they were still Quake bots.

So I expanded the archive again.

Looking back, I think client-side bots probably deserved their own archive.

They are closely related to the original topic, but they are not really Quake modifications in the same sense as server-side bots.

They form a distinct category with their own development history and technical challenges.

A dedicated client-side bot archive could have explored that history in much greater detail without complicating the scope of the original project.

Instead, I included them in the Quake Bot Archive.

I don't regret preserving the files. I'm glad they're there.

But I do think the archive would have been easier to research, organise, and maintain if I had been more disciplined about its boundaries.

## The Problem With an Interesting Subject

This is one of the dangers of archiving something you genuinely enjoy.

Everything seems interesting.

You find a project that is only loosely related to your topic, but it has a fascinating history.

You discover a modification that borrowed code from another project, and suddenly you want to preserve that project too.

You find an obscure release that raises questions about an entirely different branch of development.

Before long, you're following every interesting connection.

And there are always more connections.

I found it particularly difficult to exclude things because I knew how fragile these old files were.

If I came across a rare release of a modification, I wanted to preserve it, even if it didn't quite fit the archive.

What if I couldn't find it again?

What if the website disappeared?

What if nobody else was preserving it?

Those are reasonable concerns, but they don't necessarily mean every discovery belongs in the same archive.

You can save an interesting file without expanding the scope of your project to include the entire history of the modification it belongs to.

You can document a relationship without taking responsibility for preserving every related project.

And you can always create another archive.

That's a lesson I learned through experience.

**An interesting connection is not necessarily a good reason to expand the scope of an archive.**

## A Better Example: ThreeWave Capture the Flag

One of my later archives provides a useful contrast.

The ThreeWave CTF Archive focuses on a single, historically important Quake modification: ThreeWave Capture the Flag.

* [ThreeWave CTF Archive](https://github.com/Jason2Brownlee/ThreeWaveCTF)\
	`https://github.com/Jason2Brownlee/ThreeWaveCTF`

ThreeWave CTF was developed by Dave Kirsch, better known as *Zoid*, who later went on to work at id Software.

It helped establish Capture the Flag as a major multiplayer game mode in first-person shooters, influencing the games and communities that followed.

It's exactly the kind of project I think deserves careful preservation.

But unlike the Quake Bot Archive, the scope is extremely narrow.

The archive focuses on the original ThreeWave CTF modification and its releases.

Not every Capture the Flag modification.

Not every modification inspired by ThreeWave.

Not every Quake multiplayer modification that happened to include flags, teams, or similar gameplay.

Just ThreeWave CTF.

This makes an enormous difference.

There aren't a huge number of releases to find.

The development chronology is relatively easy to reconstruct, and there is surviving historical evidence to help establish when releases occurred and what changed between them.

I was able to track down almost every known release and assemble a reasonably complete history of the project.

The result is a focused archive of an important modification.

And, perhaps more importantly, it's an archive that feels achievable.

There are still gaps to investigate and improvements to make, as there always are with historical research. But the boundaries are clear, and the amount of work is manageable.

I can make meaningful progress toward completing it.

That's a very different experience from working on an archive whose scope keeps expanding every time I discover something interesting.

## Smaller Can Be Better

If I were starting the Quake Bot Archive again today, I would probably make some different decisions.

I might limit the main archive to modifications whose primary purpose was to provide computer-controlled opponents for Quake.

I might create a separate archive for client-side bots.

And I would probably document modifications that merely included bots as related projects, rather than attempting to preserve their complete release histories.

That would still leave a substantial amount of work.

But it would provide clearer boundaries and make the archive easier to understand, research, and maintain.

This is why I recommend choosing a narrow scope, especially for your first archive.

A small, focused archive has several advantages.

You can develop a good understanding of the entire project. You can identify most of its releases, investigate missing files, reconstruct its chronology, and support your findings with historical evidence.

You can also reach a point where the archive feels substantially complete.

That's an important and satisfying milestone.

A broad archive, on the other hand, can easily become a project with no obvious endpoint.

There is always another related modification, another release to find, another developer to investigate, or another historical connection to document.

Of course, there's nothing inherently wrong with a large archive. Some subjects genuinely require a broad scope, and a long-running archival project can be enormously rewarding.

But it's worth making that decision deliberately.

Don't let the scope expand simply because you've discovered something interesting.

## Give Yourself Permission to Stop

Perhaps the most useful lesson I learned is that you don't have to preserve everything.

You can care deeply about Quake history without taking responsibility for every modification you discover.

You can build an excellent archive of a single project, a single series of releases, or a narrowly defined category of modifications.

You can leave related projects for another day, another archive, or another archivist.

And if you eventually decide to expand your scope, you can do so consciously, with an understanding of the additional work involved.

The Quake Bot Archive taught me a great deal about researching and preserving old software.

It also taught me how easily a project can grow beyond its original intentions.

The ThreeWave CTF Archive showed me the value of doing the opposite: choosing something important, defining a clear boundary, and concentrating on preserving it as thoroughly as possible.

Both experiences have shaped how I approach new archival projects.

**My advice is simple: start small, keep your scope tight, and aim to do one thing really well.**

You can always create another archive.

And if your experience is anything like mine, you probably will.

