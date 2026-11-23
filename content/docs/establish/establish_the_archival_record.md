---
title: 7. Establish the Archival Record
weight: 30
---

# 7. Establish the Archival Record

In the previous chapter, you created a directory structure for your archive. You now have somewhere to store recovered files, research notes and information about missing releases.

The next step is to establish the archival record itself.

An archive is more than a collection of old downloads. It is a documented account of the modification, its creators, its releases and the origins of surviving files. Reconstructing this history is difficult because the evidence is rarely available in one place.

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

For example, the suggested sections in this document is provided below:

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
Examples might include team formation and mod reviews.

## Project Websites

Original project websites, developer websites,
mirrors and archived URLs.

## Historical Download Locations

Original URLs where releases and supplementary files
were distributed. These could be inline with each release.

## References

Historical sources supporting the information
in this document.
```

You do not need to fill in every section immediately. In fact, some sections might initially contain only a few lines.

The important thing is to establish the document early and update it whenever you discover something relevant.

## Create a chronology of releases

The central part of `history.md` should be a chronological account of the modification's releases.

It is useful to distinguish between a release and a file. A release represents a particular version or distribution of a modification, while a file is an actual downloadable artefact. A single release might be distributed through several files, and different files might contain identical copies of the same release. We will examine these distinctions in detail when verifying recovered files in a later chapter.

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

For example, a portion of a fictional release history might look like this:

```
## Releases and Chronology

## Version 0.1

- Files Released: ...
- Estimated Release Date: ...
- Status: Recovered

Release announcements:
...

Historical and modern download locations:
...

Metadata for each file:
...

Content of each file:
...
```

Start with whatever evidence is available. Mark unknown details clearly and update the entry as you make discoveries.

### Record the release name and version

Use the version number or release name as it appeared in the original material whenever possible.

Do not assume that filenames accurately identify versions.

For example, a file called `aq_final.zip` might contain version 1.0, while a file called `aq10.zip` might contain a later revision.

Use the readme, release announcement or other evidence to establish the version.

If the version is unknown, use a descriptive label rather than guessing.

For example: "Unidentified beta release".

You can revise this entry later if additional evidence becomes available.

### Distinguish different kinds of dates

Historical research often produces several different dates for the same release.

For example:

- The date a developer announced a release.
- The date the release was made available for download.
- The date a file was uploaded to an FTP server.
- The date a magazine CD containing the release was published.
- The modification timestamp stored inside the downloaded archive.
- The date in the release readme file.

These dates are not necessarily the same.

Suppose a modification was announced in April 1998, but a copy appears on a magazine CD published in July 1998. The magazine date does not establish the original release date.

Similarly, a ZIP file might contain files with timestamps from March 1998, but this does not necessarily prove that the ZIP itself was released in March.

Record the date that the evidence actually supports. Keep announcement, release and later distribution dates distinct rather than choosing one date to represent them all.

If you only know that a release appeared sometime during March 1998, record March 1998 without inventing a precise day. If you only know the year, record the year.

You can also distinguish between confirmed and approximate dates:

```
#### Version 1.0

- Announcement date: April 1998
  Evidence: Original project announcement.
- Download advertised by: April 1998
  Evidence: Archived download page captured in April.
- Release date: Not established precisely.
- Later distribution: July 1998
  Evidence: Magazine CD contents listing.
```

The objective is to build an accurate historical record, not to make every entry appear equally certain.

### Record filenames, file sizes and hashes

Record the original filename exactly as it was distributed.

File sizes are also useful because they can help distinguish different copies or versions of a release.

For example, two files might both be called `aq10.zip`, but have different sizes. This could indicate that one is a modified copy, an incomplete download or a different release that reused the same filename.

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

Use the `tree` or `ls -l` command on macOS or Linux to summarize an unzipped distribution of a modification or the `tar tvf` command to list the contents of an archive. This was touched on in the previous chapter.

### Record changelog information

Changelogs are often included in modification readmes or release announcements. Record significant changes for each release.

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
### Version 1.0

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

For important sources, preserve a short, relevant quotation or summary alongside the original URL, archived URL and source details. Avoid reproducing lengthy documents in `history.md`. Where useful, preserve a separate copy of the original evidence.

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

Original project websites can provide release announcements, readmes, developer information and download links. Many have disappeared, making it important to record every known website associated with the modification, including those no longer accessible.

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

Add a section to `history.md` that records historical download locations under each release.

This is different to the contents of `wishlist_urls.txt` that only includes known historical URLs for files that have not yet been recovered, whereas the historical download locations in the `history.md` include all known URLs for each given release, recovered or otherwise.

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

You might investigate the surrounding directory (directly or via the Wayback Machine on `archive.org`, more on this later):

```
/pub/quake/actionquake/
```

It could contain earlier versions, patches, maps or readme files.

A single historical URL can therefore lead to the recovery of several additional files.

Record URLs exactly as they appear in the source. Preserve the original protocol, hostname, path and filename. Do not silently correct or modernise them.

If you find a possible alternative URL, record it as a separate location.

## Update the record as you research

Update the archival record as you research, rather than leaving the work until the end.

After several weeks of searching websites, reading discussions and downloading files, it can become difficult to remember where individual discoveries came from. You might forget which website provided a filename, whether a date came from a readme or an announcement, or which URL was associated with a particular release.

For example:

**You discover a release announcement.**

- Add the announcement to `history.md`.
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
- Update the `README.md` release catalogue.

**You find a reference to a missing release.**

- Add the release to the `Releases and Chronology` section with an appropriate uncertainty status.
- Add any known filename to `wishlist.txt`.
- Record the historical download URL in `wishlist_urls.txt`, if available.

Keeping the record current also makes it easier to pause your research and resume it later without retracing your steps.

## Chapter summary

The archival record turns scattered research into an organised account of a modification's history.

The main ideas from this chapter are:

- `history.md` is the central historical record for the project.
- Maintain one chronological record of releases, including announcements, distribution dates, recovered files and supporting evidence.
- Record other significant historical events separately when they are not associated with a release.
- Record filenames, file sizes, hashes, archive contents and changelog information where available.
- Maintain lists of project websites, developer websites and mirrors.
- Preserve historical download URLs even when the original files are no longer available.
- Update the archival record as you research, rather than leaving the work until the end.

**Outcome:** You have a system for turning unstructured research into an organised historical record. Your archive now has a central place to document releases, websites, download locations, historical references and unresolved questions.

In the next chapter, you will begin researching the original project websites. You will learn how to use surviving websites and the Wayback Machine to reconstruct project histories, identify release announcements and locate files that are no longer available from their original hosts.
