---
title: 7. Establish the Archival Record
weight: 3
---

# 7. Establish the Archival Record

In the previous chapter, you created a directory structure for your archive. You now have somewhere to store recovered files, research notes and information about missing releases.

The next step is to establish the archival record itself.

This is one of the most important parts of the entire process. An archive is not simply a collection of old downloads. It is a documented account of what a modification was, who created it, what was released, when it was distributed and where the surviving files came from.

The challenge is that this information is rarely available in one place.

You might find a release announcement in an old gaming news archive, a filename in a Usenet discussion, a download link in an archived website and an actual copy of the file on a magazine CD. Each discovery contributes a small piece of the historical record.

If you do not record these discoveries systematically, you will eventually lose track of what you know, where you found it and which questions remain unanswered.

This chapter introduces a practical system for turning those scattered discoveries into an organised historical record.

## The archival record

The central document for your archive is:

```
research/history.md
```

This document should become the main account of the modification's history.

It is not intended to be a collection of informal research notes. Instead, it should contain an organised record of the project's development, releases, websites, distribution locations and supporting evidence.

You will update it throughout the research process.

A useful way to think about the document is as a combination of four things:

1. A chronological history of the project.
2. A record of other significant historical events, where relevant.
3. A record of project websites and historical download locations.
4. A collection of references supporting the historical record.

These are closely related. A release announcement might establish that a new version existed, identify its filename and provide a download URL. That single discovery could contribute information to several sections of your archival record.

You should aim to record the information once and connect it to the relevant parts of the document.

## Create the history document

Start by creating a basic structure in `research/history.md`.

For example:

```
# Project History

## Overview

A short description of the modification, its purpose
and its development.

## Releases and Chronology

A chronological account of known releases, including the evidence
that establishes when each release was announced, distributed
and recovered.

## Other Historical Events

Significant events that are not directly associated with a release.

## Project Websites

Original project websites, developer websites,
mirrors and archived URLs.

## Historical Download Locations

Original URLs where releases and supplementary files
were distributed.

## References

Historical sources supporting the information
in this document.

## Outstanding Questions

Important unresolved questions and missing information.
```

This structure gives you somewhere to record the main categories of information you will discover.

You do not need to fill in every section immediately. In fact, some sections might initially contain only a few lines.

The important thing is to establish the document early and update it whenever you discover something relevant.

## Create a chronology of releases

The central part of `history.md` should be a chronological account of the modification's releases.

Rather than maintaining a general chronology and a separate release catalogue, combine them into one section. Each release is a point in the project's history, and the evidence used to document it belongs with that release.

This avoids recording the same event twice and reduces the risk of the chronology and release catalogue becoming inconsistent.

The section should capture what was released, when it was announced or distributed, what files were involved, what changed and what evidence supports the record.

A modification might have many different types of releases:

- Public betas.
- Full releases.
- Incremental updates.
- Bug-fix patches.
- Map packs.
- Model packs.
- Server-side versions.
- Linux or other platform-specific versions.
- Source code releases.
- Unofficial updates and community modifications.

Arrange entries in chronological order, using the best-supported release date. If the date is uncertain, place the entry where it most likely belongs and make that uncertainty clear.

Record each meaningful release or distribution separately. If a patch was distributed separately from the main release, give it its own entry and connect it to the version it updates.

For example, a fictional release history might look like this:

```
## Releases and Chronology

### 1997

#### Version 0.1

- Announcement date: March 1997
- Release date: June 1997
- Status: Recovered
- Files:
  - aq01.zip
- File size: 2.4 MB
- SHA-256: [hash]
- Contents:
  - Game files
  - Three maps
  - Readme
- Changelog: Initial public release.
- Announcement: [Reference]
- Original download URL: [URL]
- Recovered from: [Source]
- Questions: None.

#### Version 0.5

- Announcement date: August 1997
- Release date: September 1997
- Status: Missing
- Files:
  - aq05.zip
- File size: Unknown
- Contents: Unknown.
- Changelog: Additional maps and weapons.
- Announcement: [Reference]
- Original download URL: [URL]
- Questions:
  - Is this a full release or a patch?
  - Does a copy survive on a magazine CD?

### 1998

#### Version 1.0

- Announcement date: March 1998
- Release date: April 1998
- Status: Recovered
- Files:
  - aq10.zip
- File size: 4.2 MB
- SHA-256: [hash]
- Contents:
  - Game files
  - Maps
  - Readme
- Changelog: First major release.
- Announcement: [Reference]
- Original download URL: [URL]
- Distribution:
  - Original project website
  - Third-party gaming magazine CD, July 1998
- Recovered from: [Source]
- Questions: None.
```

The example uses fictional information. Its purpose is to show how the release record combines the sequence of releases with the evidence for each one.

You do not need to know all these details before creating an entry. Start with what the evidence establishes, leave unknown fields blank or mark them as unknown, and update the entry as you make discoveries.

### Record the release name and version

Use the version number or release name as it appeared in the original material whenever possible.

Do not assume that filenames accurately identify versions.

For example, a file called `aq_final.zip` might contain version 1.0, while a file called `aq10.zip` might contain a later revision.

Use the readme, release announcement or other evidence to establish the version.

If the version is unknown, use a descriptive label rather than guessing.

For example:

```
#### Unidentified beta release

- Version: Unknown
- Announcement date: Unknown
- Release date: Unknown
- Filename: aq_beta.zip
- Status: Recovered
- Notes: Readme identifies the project but does
  not specify a version number.
- Evidence: [Reference]
```

You can revise this entry later if additional evidence becomes available.

### Distinguish different kinds of dates

Historical research often produces several different dates for the same release.

For example:

- The date a developer announced a release.
- The date the release was made available for download.
- The date a file was uploaded to an FTP server.
- The date a magazine CD containing the release was published.
- The modification timestamp stored inside the downloaded archive.

These dates are not necessarily the same.

Suppose a modification was announced in April 1998, but a copy appears on a magazine CD published in July 1998. The magazine date does not establish the original release date.

Similarly, a ZIP file might contain files with timestamps from March 1998, but this does not necessarily prove that the ZIP itself was released in March.

Record the date that the evidence actually supports. Keep announcement, release and later distribution dates distinct rather than choosing one date to represent them all.

If you only know that a release appeared sometime during 1998, record the year rather than inventing a precise month or day.

You can also distinguish between confirmed and approximate dates:

```
#### Version 1.0

- Announcement date: April 1998
  Evidence: Original project announcement.
- Release date: Approximately April 1998
  Evidence: Archived download page captured in April.
- Later distribution: July 1998
  Evidence: Magazine CD contents listing.
```

The objective is to build an accurate historical record, not to make every entry appear equally certain.

### Record filenames, file sizes and hashes

Record the original filename exactly as it was distributed.

File sizes are also useful because they can help distinguish different copies or versions of a release.

For example, two files might both be called `aq10.zip`, but have different sizes. This could indicate that one is a modified copy, an incomplete download or a different release that reused the same filename.

Do not assume that matching filenames mean matching files.

For recovered files, calculate a cryptographic hash such as SHA-256.

A hash provides a compact identifier for the exact contents of a file.

For example:

```
aq10.zip
Size: 4,203,112 bytes
SHA-256: 8f4c...example...a291
```

The hash shown here is illustrative.

If you recover the same file from two different locations and the SHA-256 hashes match, you have strong evidence that the files are identical.

If the hashes differ, the files are not identical, even if their filenames are the same.

This is particularly useful when comparing files recovered from magazine CDs, FTP mirrors and archived websites.

You do not need to calculate hashes for every file before starting your research. However, you should plan to include them in the relevant release entry as files are recovered and verified.

### Record the contents of distributed archives

A ZIP file may contain much more than the main modification.

For example, it might contain:

```
aq10.zip
    README.TXT
    INSTALL.TXT
    PAK0.PAK
    PAK1.PAK
    maps/
        aq_dm1.bsp
        aq_dm2.bsp
    models/
        player/
    sounds/
```

Recording the contents can help you understand what was distributed and identify differences between releases.

It can also reveal files that were distributed separately.

For example, a readme might refer to a map that is not included in the archive. This could indicate that the map was a separate download or part of a supplementary release.

Initially, a short description may be sufficient. For larger projects, you might maintain a separate file inventory.

### Record changelog information

If a release includes a changelog or readme, record the important changes.

For example:

```
Version 1.1 changes:

- Fixed weapon balance.
- Added two maps.
- Corrected multiplayer bugs.
- Updated server configuration.
```

You do not necessarily need to reproduce every changelog in `history.md`. You can summarise it and preserve or link to the original readme.

Changelogs are particularly useful for distinguishing releases and understanding how a modification evolved.

### Record the evidence for each release

For every release, record where you found evidence of its existence and what that evidence establishes.

This might include:

- An announcement on the original project website.
- A post in a gaming news archive.
- A Usenet discussion.
- A magazine CD listing.
- An FTP directory listing.
- A surviving readme.
- A later review or retrospective.

A release announcement and a download location provide different kinds of evidence. The announcement may establish when the release was made, while the download URL tells you where the file was distributed. A surviving copy establishes that a file with those contents exists, but may not by itself establish when it was originally released.

Record the source and the specific information it supports. For example:

```
#### Version 1.0

- Announcement date: April 1998
- Release date: April 1998
- Announcement evidence:
  - Example Gaming News, 12 April 1998: [Reference]
- Download evidence:
  - Archived project page, captured 15 April 1998: [Reference]
- File evidence:
  - aq10.zip recovered from a magazine CD.
- Original download URL:
  - ftp://ftp.example.invalid/pub/quake/aq10.zip
```

The references themselves should also be included in `research/lists/references.md`, as described later in this chapter. The release entry should make it clear which references support that particular release.

### Record other historical events separately

Not every important event belongs to a release entry.

Some events help explain the project's history but are not directly associated with a particular release. Examples include:

- The development team was formed.
- The project website was launched.
- A new developer joined the team.
- The project changed ownership.
- Development was discontinued.
- A successor or derivative project was announced.

Record these in an optional section after the release chronology:

```
## Other Historical Events

### 1997

- **May:** The development team is formed.
  Evidence: [Reference]

### 1998

- **January:** The project website is launched.
  Evidence: [Reference]

### 1999

- **September:** The developers announce that
  active development has ended.
  Evidence: [Reference]
```

Keep this section for events that are not already documented as part of a release. For example, do not repeat a version announcement here if it is already recorded in that version's entry.

## Maintain a list of project websites

The project website is often one of the most valuable sources of historical information.

It may contain release announcements, screenshots, readmes, developer information, download links and references to related projects.

However, many Quake modification websites have disappeared.

You should therefore maintain a list of all known websites associated with the project, including websites that no longer exist.

Add a section to `history.md`:

```
## Project Websites

### Original project website

- URL: http://www.example.invalid/
- Status: No longer available.
- Wayback Machine: [Archived captures]

### Developer website

- URL: http://developer.example.invalid/
- Status: Unknown.
- Notes: Referenced in a project readme.

### Community mirror

- URL: http://mirror.example.invalid/actionquake/
- Status: No longer available.
- Notes: Listed in an old gaming news article.
```

These are placeholder URLs.

Include more than just the main project homepage.

You might discover:

- A separate website for the development team.
- Personal websites belonging to individual developers.
- A PlanetQuake or other community-hosted project page.
- A mirror maintained by another Quake community member.
- An FTP server containing releases.
- An archived version of a website on the Wayback Machine.

Record the original URL and any archived or alternative locations separately.

A vanished website is still historically important. Its URL may appear in announcements, readmes and other websites, providing clues about where files were distributed.

Do not discard a URL simply because it no longer works.

## Maintain a record of historical download locations

Project websites and download locations are closely related, but they are not quite the same thing.

A project website might have existed at:

```
http://www.example.invalid/actionquake/
```

The actual download might have been hosted at:

```
ftp://ftp.example.invalid/pub/quake/actionquake/aq10.zip
```

You should preserve both.

Add a section to `history.md` that records historical download locations:

```
## Historical Download Locations

### Version 1.0

- Original URL:
  ftp://ftp.example.invalid/pub/quake/aq10.zip

- Archived URL:
  [Wayback Machine capture]

- Other known locations:
  http://mirror.example.invalid/aq/aq10.zip

- Current status:
  Original FTP unavailable.
  File recovered from a magazine CD.

### Version 1.1

- Original URL:
  http://www.example.invalid/files/aq11.zip

- Archived URL:
  [Wayback Machine capture]

- Current status:
  File not yet recovered.
```

Historical download URLs are valuable even when they no longer work.

They tell you:

- The original filename.
- The directory structure used by the developer.
- The server or website that hosted the release.
- The likely location of related files.
- Whether multiple mirrors existed.
- Which historical sources might contain a copy.

For example, if you find this URL:

```
ftp://ftp.example.invalid/pub/quake/actionquake/aq10.zip
```

You might investigate the surrounding directory:

```
/pub/quake/actionquake/
```

It could contain earlier versions, patches, maps or readme files.

A single historical URL can therefore lead to the recovery of several additional files.

Record URLs exactly as they appear in the source. Preserve the original protocol, hostname, path and filename. Do not silently correct or modernise them.

If you find a possible alternative URL, record it as a separate location.

## Create a catalogue of historical references

Your research will produce many sources that do not fit neatly into the release catalogue or website list.

These might include news articles, forum discussions, reviews, Usenet posts, magazine articles and FTP directory listings.

Create a separate document:

```
research/lists/references.md
```

This document is a catalogue of the historical sources you have discovered.

A useful initial structure is:

```
# Historical References

## Gaming News

## Forum Discussions

## Usenet Posts

## Reviews and Articles

## Magazine CDs

## FTP Listings

## Other Archives
```

For each reference, record enough information to find and understand it later.

For example:

```
## Gaming News

### Action Quake 1.0 announcement

- Source: Example Gaming News
- Date: April 1998
- URL: http://news.example.invalid/article123
- Archived URL: [Wayback Machine capture]
- Information:
  Announces the release of Action Quake 1.0.
- Related release: Version 1.0
```

Again, the source and release information are fictional.

A reference should ideally include:

- Source name.
- Author, if known.
- Publication or posting date.
- Original URL or location.
- Archived URL, if available.
- Short description of relevant information.
- Related release, developer or historical event.

You do not need to write a full summary of every article. A short description is usually enough to remind you why the source matters.

### Why maintain a separate reference catalogue?

Imagine that you discover 30 historical references while researching a modification.

Some mention releases, others mention developers, and several provide clues about the original website.

If you record every reference only inside the relevant release entry, you might lose sight of the broader collection of sources.

A separate reference catalogue provides a central index.

It also makes it easier to identify sources that have not yet been investigated properly.

For example, you might have a list of 15 Usenet posts but only have examined five of them. The remaining ten become obvious research tasks.

The reference catalogue also helps you avoid repeatedly rediscovering the same source.

## Connect discoveries to the relevant releases

The most important principle in maintaining the archival record is that information should be connected.

It is not enough to collect a large list of URLs, filenames and historical references. You need to establish how they relate to the project and its releases.

Consider a fictional research example.

You discover three things:

1. A gaming news article from April 1998 announces version 1.0.
2. A Wayback Machine capture from the same month contains a download link to `aq10.zip`.
3. A copy of `aq10.zip` is found on a magazine CD.

These discoveries should be connected.

The news article is added to `research/lists/references.md`.

The original download URL is recorded in the historical download locations section of `history.md`.

The recovered file is placed in `bin/`, and its filename, size, hash and contents are recorded in the version 1.0 entry.

The April 1998 release entry is updated with the announcement, download URL and recovery evidence.

The result is a connected historical record:

**Example: Connecting historical discoveries**

**Gaming news article**

April 1998

Announces version 1.0.

**Historical download URL**

Original project website

Identifies `aq10.zip` and its original location.

**Recovered file**

Magazine CD

Provides a surviving copy of `aq10.zip`.

**Version 1.0 archival record**

history.md

Connects the release date, announcement, original URL, recovered file and supporting evidence.

This is the difference between collecting information and conducting archival research.

Each discovery should help establish or clarify something about the modification.

You should also record the source of each claim. If you later discover that the news article was referring to a beta rather than the final release, you can revisit the evidence and correct the record.

## Record uncertainty and outstanding questions

Historical research is rarely complete.

You will encounter missing files, conflicting dates, unidentified versions and references that cannot be independently verified.

Do not hide these problems or silently turn uncertain information into facts.

Record them explicitly.

For example:

```
## Outstanding Questions

### Version 0.7

- A December 1997 forum post mentions this version.
- No surviving download has been found.
- It is unclear whether this was a public release
  or a private development build.

### Original homepage

- The original URL is known.
- No working copy has been located.
- Wayback captures begin several months after
  the first public release.

### Developer identity

- A readme credits "John".
- It is unclear whether this refers to John Smith,
  who is credited on a later release.
```

Some of these questions might eventually be resolved. Others might remain unanswered indefinitely.

You can also use status labels such as:

- **Confirmed:** Directly supported by reliable evidence.
- **Probable:** Supported by evidence, but not fully established.
- **Unverified:** Mentioned in a source but not independently confirmed.
- **Speculative:** A possible explanation or research lead.
- **Unknown:** No reliable information currently available.

The important thing is consistency.

If you use these labels, make sure they mean the same thing throughout your research documents.

## Update the record as you research

You should not wait until the end of your research to write the historical record.

This is a surprisingly easy mistake to make.

You might spend several weeks searching old websites, reading forum discussions and downloading files. You collect dozens of browser bookmarks and save a few notes in different places.

Eventually, you decide to organise everything.

By then, you might no longer remember which website provided a particular filename, whether a date came from a readme or a news article, or which download URL was associated with a particular release.

Instead, update the archival record whenever you make a useful discovery.

For example:

**You discover a release announcement.**

- Add the announcement to `research/lists/references.md`.
- Add or update the release entry in the `Releases and Chronology` section of `history.md`.
- Record any filenames or download URLs mentioned in the announcement.

**You find an archived project homepage.**

- Add the original URL to the project websites section.
- Record the Wayback Machine URL and capture date.
- Extract useful release information and add it to the relevant entries.
- Record any new questions or leads in `notes.txt`.

**You recover a ZIP file.**

- Place the original file in `bin/`.
- Record its filename and source.
- Calculate its size and SHA-256 hash.
- Inspect its contents.
- Connect it to the appropriate release entry.
- Update the README release catalogue.

**You find a reference to a missing release.**

- Add the release to the `Releases and Chronology` section with an appropriate uncertainty status.
- Add any known filename to `wishlist.txt`.
- Record the historical download URL in `wishlist_urls.txt`, if available.
- Add the source to `research/lists/references.md`.

This process ensures that your archival record develops alongside your research.

It also means that you can stop working at any point and return later without having to reconstruct everything you discovered.

## A practical example: Starting an archival record

Suppose you have chosen to archive a fictional Quake modification called *Shadow Arena*.

You have found three pieces of information:

- A 1997 news article announcing the modification.
- An archived project homepage with a link to `shadow01.zip`.
- A forum discussion mentioning a later version called 1.2.

You have not yet recovered any files.

Your initial archival record might look like this:

```
# Shadow Arena History

## Overview

Shadow Arena was a multiplayer modification
for Quake. Its development began in 1997.

## Releases and Chronology

### 1997

#### Initial release

- Version: Unknown
- Date: Approximately June 1997
- Filename: shadow01.zip
- Status: Missing
- Original download URL:
  http://example.invalid/files/shadow01.zip
- Evidence: Archived project homepage.
- Questions: Exact version number unknown.

#### Version 1.2

- Date: Unknown
- Filename: Unknown
- Status: Unverified
- Evidence: Forum discussion.
- Questions: Was this a public release?

## Project Websites

- Original homepage:
  http://example.invalid/
- Archived homepage:
  [Wayback Machine capture]

## Historical Download Locations

- http://example.invalid/files/shadow01.zip

## Outstanding Questions

- Can the initial release be recovered?
- Did version 1.2 receive a public download?
- Who were the original developers?
```

Even though you have not recovered a single file, you already have the beginnings of a useful archive.

You know that the project existed, have a possible release filename, have an original download location and have a reference to a later version.

You also know what remains uncertain.

This is a meaningful result. It gives you a starting point for the next stage of research.

## Your archival record checklist

Before moving on, make sure your archive has a place for each of the following:

- A chronological record of releases and their supporting evidence.
- A record of other significant historical events, where relevant.
- Version numbers or release names.
- Known release dates and date uncertainty.
- Original filenames and file sizes.
- File hashes where available.
- Contents of recovered archives.
- Changelog information.
- Release announcements and supporting evidence.
- Original project and developer websites.
- Historical download URLs.
- A catalogue of other historical references.
- Outstanding questions and missing information.

You do not need to have all this information yet. The purpose is to establish a system that can accommodate it as you make discoveries.

## Chapter summary

The archival record turns scattered research into an organised account of a modification's history.

The main ideas from this chapter are:

- `history.md` is the central historical record for the project.
- Maintain one chronological record of releases, including announcements, distribution dates, recovered files and supporting evidence.
- Record other significant historical events separately when they are not associated with a release.
- Record filenames, file sizes, hashes, archive contents and changelog information where available.
- Maintain lists of project websites, developer websites and mirrors.
- Preserve historical download URLs even when the original files are no longer available.
- Use `research/lists/references.md` to catalogue news articles, forum discussions, Usenet posts, reviews, FTP listings and other sources.
- Connect every discovery to the relevant release or historical event.
- Record uncertainty and outstanding questions rather than guessing.
- Update the archival record as you research, rather than leaving the work until the end.

**Outcome:** You have a system for turning unstructured research into an organised historical record. Your archive now has a central place to document releases, websites, download locations, historical references and unresolved questions.

In the next chapter, you will begin researching the original project websites. You will learn how to use surviving websites and the Wayback Machine to reconstruct project histories, identify release announcements and locate files that are no longer available from their original hosts.