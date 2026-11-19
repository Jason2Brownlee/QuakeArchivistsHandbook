---
title: 8. Research Original Project Websites
weight: 1
---

# 8. Research Original Project Websites

In the previous chapter, you established a system for recording the history of a modification, documenting its releases and connecting discoveries to supporting evidence.

You are now ready to begin researching.

One of the best places to start is the original project website.

During the Quake modding era, developers commonly maintained their own websites to announce updates, distribute files, publish screenshots, provide installation instructions and communicate with their communities. Some projects had dedicated websites, while others were hosted on personal pages, community portals or gaming sites.

These websites can be extremely valuable historical sources. They often provide direct evidence of what was released, when it was released, what files were distributed and where those files were hosted.

Unfortunately, many of these websites no longer exist. The original domain may have expired, the hosting provider may have disappeared, or the developer may have moved on to other projects.

This does not necessarily mean the information is lost.

The Internet Archive's Wayback Machine has preserved snapshots of many historical websites. Even when a website is no longer available, you may be able to recover its pages, follow old links and discover references to files that survive elsewhere.

This chapter explains how to find original project websites, investigate their archived versions and extract useful information for your archive.

## Find the original project website

Your first task is to identify the websites associated with the modification.

Start with the information you already have. Your research notes, release announcements, readme files and historical references may contain the original project URL.

Look for references such as:

- The project homepage.
- A developer or team website.
- A download page.
- A community-hosted project page.
- A news page maintained by the developers.
- A personal website belonging to one of the contributors.

Do not assume that the first website you find is the original project homepage. A modification might have been hosted on several different websites over its lifetime.

For example, a project could have started on a developer's personal website, moved to a dedicated domain and later been mirrored by a Quake community portal.

Record each relevant URL in the project websites section of `research/history.md`.

For each website, capture:

- The original URL.
- The website's apparent purpose.
- Its relationship to the project.
- Whether it is still accessible.
- Any archived versions you find.
- Where you found the URL.

If you do not yet know the original URL, search for the modification's name together with terms such as `homepage`, `official site`, `download`, `Quake mod` and the developer's name.

Old readme files and release announcements are particularly useful because they often include the project's official website and download locations.

You should also search for variations of the project name. A modification might have been referred to by a shortened name, an acronym or an earlier working title.

The goal at this stage is to build a list of candidate websites, not to decide that one particular site contains the complete history.

## Use the Internet Archive's Wayback Machine

The Internet Archive operates the [Wayback Machine](https://web.archive.org/?utm_source=chatgpt.com), a service that stores historical captures of websites.

It is one of the most important tools for researching old Quake modifications.

A website that disappeared in 2002 might still have captures from 1998, 1999 and 2001. These captures can preserve homepage text, news announcements, download pages, screenshots and links to files.

The Wayback Machine does not necessarily preserve every page or every file. Some captures are incomplete, and links may no longer work. Nevertheless, it is often possible to reconstruct a substantial amount of a project's original website.

### Inspect the capture history for a domain

Open the Wayback Machine and enter the original project URL.

For example:

```
http://www.example.invalid/
```

The Wayback Machine will show a calendar or timeline indicating when captures are available.

The capture history gives you an overview of how much of the website was preserved and when snapshots were taken.

Look for:

- The earliest available capture.
- Captures around known release dates.
- Periods when the website was updated frequently.
- Long gaps between captures.
- The final captures before the website disappeared.

The earliest capture can be useful for understanding the original project description. Later captures may contain new release announcements, updated download links or changes to the development team.

Do not assume that the earliest capture is the first version of the website. The site may have existed for months or years before the Internet Archive first captured it.

Likewise, a capture date is not necessarily the date the page was written or the information was published. It tells you when the Internet Archive saved a copy.

Record useful capture URLs and dates in your research notes or reference catalogue.

### Compare captures from different dates

A website might have been captured many times over several years.

Open captures from different dates and compare their contents.

For example, the homepage might show:

- March 1998: Version 0.5 is the latest release.
- June 1998: Version 1.0 is announced.
- October 1998: Version 1.1 is available.
- February 1999: Development of version 2.0 is underway.

Comparing captures can help establish when information appeared on the website and how the project evolved.

It can also reveal changes that are not obvious from any single capture.

For example, a download link might point to `aq10.zip` in one capture and `aq11.zip` in a later capture. The change provides a useful lead about the release sequence.

Be careful not to treat the capture dates as exact release dates. Use the page content to establish what the developer actually announced, and record the capture date as supporting evidence.

## Navigate archived versions of the website

Once you have found a useful capture, investigate the rest of the archived website.

Do not stop at the homepage.

The homepage may link to separate pages for downloads, news, screenshots, documentation, development information and frequently asked questions.

These pages can contain much more useful historical information than the homepage itself.

Look for navigation links such as:

- News.
- Updates.
- Downloads.
- Files.
- Releases.
- Screenshots.
- About.
- Team.
- Documentation.
- FAQ.
- Links.

Follow these links within the archived website.

Sometimes the Wayback Machine will successfully load the archived version of the linked page. In other cases, the page may be missing or the link may lead to an unavailable capture.

If a link fails, do not immediately assume the page was never archived. Try entering the destination URL directly into the Wayback Machine.

For example, suppose the homepage links to:

```
http://www.example.invalid/downloads.html
```

Enter that exact URL into the Wayback Machine to see whether it has its own capture history.

You can also inspect the capture history for specific directories within the project website.

For example:

```
http://www.example.invalid/
http://www.example.invalid/news/
http://www.example.invalid/files/
http://www.example.invalid/downloads/
```

A project might have a captured homepage but no captured download page, or the reverse. Investigating individual paths can reveal pages that are not obvious from the main website.

### Find all archived pages within a project directory

The Wayback Machine's capture interface is useful for examining known URLs, but it is not always convenient for discovering every page that was archived.

The Internet Archive also provides a CDX server interface that can list captured URLs for a domain or URL prefix.

For example, you can open this address in your browser:

```
https://web.archive.org/cdx/search/cdx?url=example.invalid/*
&output=json
```

This is a request for archived URLs matching the specified domain pattern. Replace `example.invalid` with the actual domain.

The results can reveal pages and files such as:

```
http://www.example.invalid/
http://www.example.invalid/news.html
http://www.example.invalid/downloads.html
http://www.example.invalid/files/aq10.zip
http://www.example.invalid/files/aq11.zip
http://www.example.invalid/screenshots/shot01.jpg
```

This can be particularly useful when the original website had many pages or when its navigation links are incomplete.

The CDX interface has additional query options for filtering results, including by URL pattern, file type and capture status. You do not need to learn all of these options immediately. Start by using it to discover the archived URLs associated with a project.

Treat the results as a list of research leads. A URL appearing in the index does not guarantee that its archived content can be retrieved successfully.

## Read homepage content and news pages

Once you have located the archived pages, read them carefully and extract information relevant to the project's history.

The homepage is often a good starting point. It may describe the modification, identify its developers, explain its features and provide links to the latest release.

News and updates pages are especially valuable. Developers often used them to announce new versions, report progress, thank contributors and explain changes.

Look for statements such as:

- "Version 1.0 is now available."
- "The first public beta has been released."
- "A new map pack is available for download."
- "The server files have been updated."
- "Development has moved to a new website."
- "The project is no longer being maintained."

Each statement can help establish an event in the project's history.

For every useful announcement, record:

- The date shown on the page.
- The version or release name.
- What the announcement says was released.
- Any filenames mentioned.
- Any download links.
- The developers or contributors mentioned.
- The archived page URL and capture date.

For example, you might find this announcement on an archived news page:

```
April 12, 1998

Action Quake 1.0 released!

The first public version of Action Quake is now
available. This release includes five new maps,
updated weapons and improved multiplayer support.

Download: aq10.zip
```

You could record the discovery in `research/history.md`:

```
#### Version 1.0

- Announcement date: 12 April 1998
- Release date: April 1998
- Filename: aq10.zip
- Contents: Five maps, updated weapons and
  multiplayer improvements.
- Announcement evidence:
  Archived project news page, captured
  15 April 1998: [URL]
- Original download URL: [URL]
- Status: File not yet recovered.
```

The example is fictional.

Notice that you have learned several things even though you have not recovered the file. You have a release name, an approximate release date, a filename, a description of the contents and a source supporting the information.

This is exactly the kind of discovery you want to capture.

### Look for information beyond release announcements

News pages can contain other useful details.

For example, a developer might announce that a new team member has joined, that the project has moved to a different website, or that a particular map was contributed by another community member.

These details can help you identify developers, related projects and additional research leads.

Record important events that are not associated with a release in the optional `Other Historical Events` section of `history.md`.

Avoid copying large amounts of website text into your historical record. Summarise the relevant information and preserve the source URL so that someone else can inspect the original evidence.

## Find download links and historical file locations

Download pages are among the most valuable parts of an original project website.

They can identify releases that are no longer available and reveal where the developers originally distributed their files.

Look for links to:

- ZIP archives.
- PAK files.
- Map packs.
- Model and texture packs.
- Patches and updates.
- Server files.
- Source code.
- Readme files.
- Installation instructions.
- Screenshots and promotional material.

Record the original URL exactly as it appears in the archived page.

For example:

```
http://www.example.invalid/files/aq10.zip
```

Do not replace this with the Wayback Machine URL. The original URL and the archived URL serve different purposes.

The original URL tells you where the developer intended the file to be downloaded. The archived URL identifies a preserved copy of the page or file, if one exists.

Your release entry might look like this:

```
#### Version 1.0

- Filename: aq10.zip
- Original download URL:
  http://www.example.invalid/files/aq10.zip
- Archived download URL:
  [Wayback Machine URL]
- Announcement:
  [Archived news page]
- Status: Not yet recovered.
```

If the download link points to another website or FTP server, record that location as well. Do not assume that every file was hosted on the project's own domain.

### Investigate archived download links

Sometimes the Wayback Machine has preserved the downloadable file itself.

Click the download link in the archived page. If the file was captured, the Wayback Machine may serve the archived copy.

If the link does not work, try entering the original file URL directly into the Wayback Machine.

For example:

```
http://www.example.invalid/files/aq10.zip
```

You can also check the capture history for the exact file URL. A file may have been captured independently of the page that linked to it.

There are several possible outcomes:

1. The archived file is available and can be downloaded.
2. The file appears in the capture index but cannot currently be retrieved.
3. The download page survives, but the file itself was never captured.
4. The original link points to an external server that was not archived.
5. The file URL is known, but there is no evidence that it was ever captured.

Record which situation applies.

Do not assume that a file is available simply because an archived page contains a download link. The page and the file are separate archival objects.

### Look for files by their URL and filename

The CDX interface introduced earlier can also help identify archived downloadable files.

You can search for a particular file extension or directory path.

For example, a project directory might contain:

```
/files/aq01.zip
/files/aq05.zip
/files/aq10.zip
/files/aq11.zip
/files/aq_patch.zip
```

This list could reveal releases that are not mentioned on the surviving homepage.

You might also discover files with less obvious names:

```
/files/aqfinal.zip
/files/aqbeta2.zip
/files/aqmaps.zip
/files/aqserver.zip
```

Record every plausible file URL, even if the file cannot be recovered.

Add missing files to `research/wishlist.txt` and their original URLs to `research/wishlist_urls.txt`, following the structure established in the previous chapters.

A historical download URL is valuable evidence in its own right. It gives you a filename and a location to investigate in later research.

## Find changelogs, readme files and documentation

Original project websites sometimes contain documentation that was distributed separately from the main modification.

Look for pages and downloads labelled:

- Readme.
- Changelog.
- History.
- Installation.
- Manual.
- Documentation.
- Frequently Asked Questions.
- Credits.

These documents can provide information that is not present in release announcements.

A readme might identify the exact version number, list the files included in a release, describe installation requirements and credit the developers.

A changelog can establish the differences between versions.

For example:

```
Action Quake 1.1

Changes since version 1.0:

- Added two new maps.
- Fixed a weapon selection bug.
- Updated player models.
- Improved server configuration.
```

This information helps distinguish version 1.1 from version 1.0 and provides a record of how the modification evolved.

If you find a readme or changelog on an archived website, preserve the original file if it can be downloaded. If it is only visible as part of an archived webpage, record the page URL and capture date.

When you later recover the corresponding ZIP file, compare its contents with the website documentation. This may help establish whether the file is the expected release.

## Identify mirrors and other distribution sites

Original project websites frequently linked to alternative download locations.

This was common when files were large, server capacity was limited or developers wanted to make downloads available through several community sites.

A download page might contain links such as:

```
Primary download:
ftp://ftp.example.invalid/pub/quake/aq10.zip

Mirror 1:
http://mirror1.example.invalid/aq10.zip

Mirror 2:
http://quake.example.invalid/files/aq10.zip
```

Record each location separately.

A mirror might have disappeared, but its URL can provide another research lead. The same file may have been preserved by a different archive, magazine CD or community member.

Also look for links to:

- PlanetQuake pages.
- Quake community websites.
- Gaming news sites.
- Mod download directories.
- Developer FTP servers.
- Personal FTP accounts.
- Other project websites.

Some of these sites may have their own archived histories. A link from the original project homepage can therefore lead you to another source of release information or surviving files.

Record the relationship between the project and the linked site. For example, distinguish a developer-maintained download location from an independent mirror.

Do not treat every linked website as an official project website. The purpose of this research is to establish what each site was and how it was connected to the modification.

## Find related projects by the same developers

The original project website may identify the people who created the modification.

Look for names and aliases in:

- Homepage credits.
- Readme files.
- News announcements.
- Team pages.
- Changelogs.
- Documentation.
- Links pages.

Record developer names and aliases carefully. A person might have used a real name in one place and a handle in another.

Once you have identified developers, look for other projects associated with them.

For example, a developer might have worked on:

- Another Quake modification.
- A map pack.
- A standalone game.
- A utility or editing tool.
- A later project for Quake II or Quake III.
- A project with a different development team.

These connections can help you discover additional material and understand the wider history of the people involved.

A developer's later project might even contain references to their earlier Quake work.

Record related projects as research leads. Do not automatically include them in your archive. Whether they belong within the archive depends on the scope you defined in Chapter 1.

## Investigate developers' personal websites

A developer's personal website can be just as useful as the original project homepage.

In the late 1990s, many developers maintained personal websites containing information about their programming, mapping, artwork and other projects.

A personal website might include:

- A portfolio of Quake maps or models.
- Links to previous projects.
- Development notes.
- Source code.
- Screenshots.
- Downloadable utilities.
- Credits and acknowledgements.
- Contact information or biographical details.

These websites can help establish who contributed to a modification and identify other work they created.

Start with the names and aliases you collected from the project website.

Search for each name together with terms such as `Quake`, `mod`, `mapping`, `programming` and the project name.

If you find a likely personal website, inspect it using the same process as the original project website:

1. Record the original URL.
2. Check its capture history in the Wayback Machine.
3. Inspect the homepage and project pages.
4. Look for references to the modification.
5. Identify other projects and contributors.
6. Record useful pages and downloadable files.

Be cautious when connecting people to projects. Similar usernames do not necessarily belong to the same person. Look for supporting evidence such as matching credits, email addresses, personal links or explicit statements.

The objective is to document the connection, not to guess at someone's identity.

## Compare findings and identify gaps

After investigating the website, review what you have found and consider what might be missing.

A website can have many archived captures, but those captures may not provide a complete history.

For example:

- The homepage survives, but the news page does not.
- A release announcement survives, but its download link is missing.
- A download page lists three versions, but only one file was captured.
- The website mentions a map pack that is not included in the available downloads.
- A later capture refers to an earlier release that does not appear in any surviving page.
- The website links to a developer's personal page, but that page has no archived captures.

These gaps are useful research information.

Record them in `research/notes.txt` or the relevant release entry in `history.md`. Add missing files to your wishlist and preserve any known URLs.

You should also compare information from different captures.

Suppose you find the following:

| Capture       | Information                                             |
| ------------- | ------------------------------------------------------- |
| March 1998    | Version 0.5 is listed as the latest release             |
| June 1998     | Version 1.0 is announced                                |
| October 1998  | Version 1.1 is available                                |
| February 1999 | Version 2.0 is mentioned, but no download link survives |

You now have a likely release sequence, but you still need to establish whether all these releases were publicly distributed and whether any files survive.

The next research chapters will help you investigate these questions using other historical sources.

## Record your discoveries

As you investigate original websites, update the archival record rather than leaving all the work until later.

The previous chapter established the main documents for this process.

Use them consistently:

| Discovery                              | Where to record it                                        |
| -------------------------------------- | --------------------------------------------------------- |
| Original project URL                   | `research/history.md`                                     |
| Archived website captures              | `research/history.md` and `research/lists/references.md`  |
| Release announcements                  | Relevant release entry in `history.md`                    |
| Release dates and version numbers      | Relevant release entry in `history.md`                    |
| Original download URLs                 | Relevant release entry and `wishlist_urls.txt` if missing |
| Recovered files                        | `bin/` and the relevant release entry                     |
| Readmes and changelogs                 | Relevant release entry                                    |
| Developer websites                     | `research/history.md`                                     |
| Related projects                       | `research/notes.txt`                                      |
| Missing files and unresolved questions | `research/wishlist.txt` and `research/notes.txt`          |

For each useful archived page, preserve enough information for someone else to find it again.

At a minimum, record:

- The original URL.
- The Wayback Machine URL.
- The capture date.
- The information you extracted.
- The related release or developer.

For example:

```
Source: Original Action Quake news page

Original URL:
http://www.example.invalid/news.html

Archived URL:
https://web.archive.org/web/19980415000000/
http://www.example.invalid/news.html

Capture date: 15 April 1998

Information:
Announces version 1.0 and identifies the
download filename as aq10.zip.

Related release:
Version 1.0
```

The example uses fictional information.

Preserve important pages and downloadable evidence where possible, following the approach established in Chapter 3. A Wayback Machine URL is useful, but it should not be your only record of an important discovery. Archived pages and files can sometimes become inaccessible or behave differently over time.

## A practical example: Researching an original project website

Suppose you are archiving a fictional Quake modification called *Shadow Arena*.

You have found an old reference to its original homepage:

```
http://shadowarena.example.invalid/
```

You enter the URL into the Wayback Machine and discover captures from 1997, 1998 and 1999.

You investigate the available captures and make the following discoveries:

**March 1997 capture**

The homepage describes Shadow Arena as a multiplayer modification for Quake. It identifies two developers and links to a news page.

**June 1997 capture**

The news page announces the first public beta. It identifies the filename as `shadow01.zip`.

**September 1997 capture**

A later news item announces version 0.5. The download page links to `shadow05.zip`, hosted on an external FTP server.

**April 1998 capture**

The homepage announces version 1.0. A changelog lists several new maps and updated weapons.

**October 1998 capture**

The download page has been updated with version 1.1. It also links to a community mirror.

**February 1999 capture**

A news item mentions that development has stopped.

You have also found an archived developer website containing a reference to another Quake project.

You have not recovered any files yet, but you have reconstructed much of the project's public-facing history.

Your archival record might now contain:

```
# Shadow Arena History

## Overview

Shadow Arena was a multiplayer modification
for Quake, developed by two contributors.

## Releases and Chronology

### 1997

#### Initial public beta

- Announcement date: June 1997
- Release date: Unknown
- Filename: shadow01.zip
- Status: Missing
- Original download URL: Unknown
- Evidence: Archived project news page.
- Questions: Where was the file hosted?

#### Version 0.5

- Announcement date: September 1997
- Release date: September 1997
- Filename: shadow05.zip
- Status: Missing
- Original download URL:
  ftp://ftp.example.invalid/shadow05.zip
- Evidence: Archived news and download pages.

### 1998

#### Version 1.0

- Announcement date: April 1998
- Release date: April 1998
- Filename: Unknown
- Status: Missing
- Contents:
  - Additional maps
  - Updated weapons
- Evidence: Archived homepage and changelog.

#### Version 1.1

- Announcement date: October 1998
- Release date: October 1998
- Filename: Unknown
- Status: Missing
- Distribution:
  - Original project website
  - Community mirror
- Evidence: Archived download page.

## Other Historical Events

### 1999

- February: Development is reported to have ended.
  Evidence: Archived project news page.

## Project Websites

- Original project homepage:
  http://shadowarena.example.invalid/
- Developer website:
  http://developer.example.invalid/

## Historical Download Locations

- ftp://ftp.example.invalid/shadow05.zip
- Community mirror: [Original URL]

## Outstanding Questions

- Can any of the missing releases be recovered?
- What was the filename for version 1.0?
- Was version 1.1 distributed on a magazine CD?
- Can the developers' other Quake projects be identified?
```

The example is fictional.

This is a substantial result. You have established a release sequence, identified developers, discovered historical download locations and identified several missing files.

You have also generated new research leads. The FTP server, community mirror and related developer project can all be investigated in subsequent chapters.

This illustrates why original project websites are such a valuable starting point. A single surviving homepage can lead to a much broader investigation.

## Your original website research checklist

Before moving on, make sure you have investigated the available original project websites and recorded your findings.

- Identified the original project homepage, where possible.
- Recorded other known project and developer websites.
- Inspected the Wayback Machine capture history for each domain.
- Examined captures around known release dates.
- Investigated news, download and documentation pages.
- Compared different captures of important pages.
- Looked for release announcements and version numbers.
- Recorded announcement dates and release dates separately.
- Recorded original filenames and download URLs.
- Checked whether downloadable files were archived.
- Looked for changelogs, readmes and installation instructions.
- Identified links to mirrors and other distribution sites.
- Investigated developers and their personal websites.
- Looked for related projects by the same developers.
- Recorded missing pages, files and other research gaps.
- Updated `history.md`, `research/lists/references.md` and your research notes.

You do not need to find every page or recover every file. The objective is to investigate the available evidence systematically and record what you discover.

## Chapter summary

Original project websites are among the best sources for reconstructing the history of a Quake modification.

They can reveal what was released, when it was announced, what files were distributed, who created the project and where the downloads were hosted.

The main ideas from this chapter are:

- Identify the original project homepage and other websites associated with the modification.
- Use the Wayback Machine to inspect archived versions of historical websites.
- Examine capture histories and compare pages from different dates.
- Follow links to news, downloads, documentation and other project pages.
- Use the CDX interface to discover archived pages and downloadable files.
- Record release announcements, dates, version numbers, filenames and changelog information.
- Preserve original download URLs, even when the files are no longer available.
- Investigate mirrors, related projects and developers' personal websites.
- Record evidence and research gaps in your archival documents.

**Outcome:** You can investigate original project websites and use their surviving content to reconstruct much of a modification's public-facing history. You can identify releases, find historical download locations, discover developers and record evidence that will guide your remaining research.

In the next chapter, you will investigate gaming news archives. These can provide another perspective on a modification's history, including release announcements, reviews, interviews and references to files that may no longer be available from the original project website.