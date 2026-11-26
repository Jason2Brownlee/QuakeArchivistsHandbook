---
title: "Interlude: Building My Own Quake Search Engine"
weight: 101
---

# Interlude: Building My Own Quake Search Engine

After years of researching Quake modifications and creating archives, I've found myself doing something I never really intended.

I've started building my own search engine for Quake files.

It happened gradually.

Every new archival project involved searching many of the same places. I'd revisit old Quake websites, browse archived FTP servers, search magazine CDs, and look through modern file mirrors.

Eventually, I started wondering why I was doing the same work over and over again.

Why not index these resources once and reuse the results for every future project?

So that's what I started doing.

## Indexing Everything

Over the years, I've written scripts to download and index enormous amounts of Quake-related material.

I've downloaded archived copies of popular Quake websites, news sites, and modification websites from the Wayback Machine, extracting every URL I could find.

I've downloaded third-party Quake CD-ROM collections from the Internet Archive and indexed their contents.

I've also indexed modern Quake file mirrors, archives, and other collections.

My focus is generally on collecting filenames and URLs, particularly historical download locations where Quake files were once available.

I don't necessarily download or preserve every file I discover. Instead, I record where files are, or where they used to be.

All these URLs go into a large database.

When I start researching a new modification, I can search that database before going back to the web.

Often, I'll immediately find historical download locations, references to old releases, or filenames that would otherwise have taken hours to discover.

It's become a useful head start for every new archival project.

## A Collection of Scripts

The system has grown into a rather messy collection of Python scripts.

Some scripts crawl websites and add newly discovered URLs to the database.

Others search the database in different ways, looking for particular filenames, directories, or patterns.

I have a simple web interface that lets me search the collected URLs.

![My custom Quake research tool for searching indexed historical file URLs.](/QuakeArchiveSearch.png)\
_Figure: My custom Quake research tool for searching indexed historical file URLs._

One script runs continuously in the background, crawling archived webpages from the Wayback Machine, extracting links, and adding them to the database.

Another script, which I run every few weeks (or days), checks the wishlist files across all my Quake archives to see whether the database contains any newly discovered historical download locations.

That last one is particularly useful.

A URL discovered while researching one modification might turn out to be exactly what I need for a completely different archive.

And because everything is indexed in one place, those discoveries aren't lost.

I should admit that much of this system is a collection of hastily assembled, vibe-coded scripts.

It's not particularly elegant. There are overlapping tools, experimental ideas, and plenty of rough edges.

But it works.

And it saves me from repeatedly searching the same collections.

## Quake Archive Search

I've made the project publicly available on GitHub:

* [Quake Archive Search](https://github.com/Jason2Brownlee/QuakeArchiveSearch)\
	`https://github.com/Jason2Brownlee/QuakeArchiveSearch`

The repository contains the scripts and tools I've developed, although it doesn't include the database itself, which has grown to more than 20 GB.

Perhaps you'll find something useful there, or at least get some ideas for building your own indexing tools.

**Perhaps I can search the index for some files that you're looking for?** Reach out any time, my contact details are at the end of the book.

I think there's real value in maintaining a searchable record of the resources you've already investigated, particularly if you intend to create multiple archives.

It doesn't need to be a large database or an elaborate collection of scripts. Even a simple text file containing discovered URLs can save a surprising amount of repeated work.

Of course, you could also argue that I've taken this a little too far.

I've spent a great deal of time building tools to help me find Quake files, time that could have been spent researching individual modifications.

Perhaps this entire system is overkill.

But after years of archival research, I've found that **the most valuable resource I've accumulated isn't necessarily the files I've recovered, but the knowledge of where to look for them.**

And having that knowledge searchable makes starting the next archive just a little bit easier.

