---
title: 8. Research Original Project Websites
weight: 10
---

# 8. Research Original Project Websites

In the previous chapter, you established a system for recording the history of a modification, documenting its releases and connecting discoveries to supporting evidence.

You are now ready to begin researching.

One of the best places to begin researching a Quake modification is its original project website.

During the Quake modding era, developers used dedicated websites, personal homepages and community portals to announce releases, distribute files and communicate with players. These pages often contain some of the best surviving evidence of the project's development and distribution history.

Although many original websites have disappeared, the Internet Archive's Wayback Machine may have preserved their content, allowing you to reconstruct the website and discover references to missing files.

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

For example, a project could have started on a developer's personal website, moved to a dedicated domain and later been migrated to a Quake community portal. In fact, a progression like this is common.

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

The Internet Archive operates the Wayback Machine, a service that stores historical captures of websites.

* [Wayback Machine](https://web.archive.org/)\
  `https://web.archive.org/`

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

## Navigate archived versions of the website

Once you find a useful capture, explore the rest of the archived website. Important information may be spread across separate pages for downloads, news, documentation and development updates.

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

### Be Careful With Websites That Use Frames

Some older websites, particularly those from the 1990s and early 2000s, used an HTML feature called *frames*. If you were browsing Quake websites back then, you'll probably remember them.

Frames allowed a website to display multiple HTML pages within a single browser window. For example, a website might have a navigation menu on the left and a main content area on the right. Clicking a link in the navigation menu would load a different page into the content area without reloading the entire website.

The important detail is that **each frame loads a separate HTML page with its own URL**.

This can cause confusion when browsing archived websites because the Wayback Machine captures each URL independently. You might be viewing a homepage from 1998 alongside a downloads page captured in 1999, potentially giving a misleading picture of which releases were available at the time.

**Don't assume that pages displayed together in a framed website were archived at the same time.**

Instead, identify the original URLs of individual frames, particularly news and download pages, and investigate their capture histories separately. This may reveal earlier or later versions of pages that are inaccessible through the archived homepage.


### Find All Archived Pages Within a Project Directory

The Wayback Machine can reveal archived URLs that no longer appear in a website's navigation.

Use the **URLs** view in the Wayback Machine to examine the pages and files captured from a particular domain or directory.

For example:

* `https://web.archive.org/web/*/example.com*`

Replace `example.com` with the historical website you are investigating.

This can reveal forgotten download pages, old news archives, files and directories that are otherwise difficult to discover.

For more extensive investigations, the Wayback Machine provides a CDX API that allows you to enumerate and filter archived URLs programmatically. We will explore this in Chapter 21, *Advanced Research Tips*.

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

A surviving announcement can establish valuable release details even when the original downloadable file is missing.

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

Preserve the original URL rather than replacing it with its Wayback Machine equivalent.

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

A developer may have worked on other Quake modifications, maps, editing tools or later projects for Quake II and Quake III. These connections can reveal additional material, including references to earlier work that might otherwise be difficult to locate.

Record related projects as research leads. Do not automatically include them in your archive. Whether they belong within the archive depends on the scope you defined earlier.

## Investigate developers' personal websites

A developer's personal website can be just as useful as the original project homepage.

In the late 1990s, many developers maintained personal websites containing information about their life, online or otherwise. Personal homepages were typically hosted on free hosting provided by domestic internet service providers or free website hosts.

A personal website might include:

- A portfolio of projects.
- Links to friends.
- Bookmarks links
- Contact information or biographical details.

These websites can can sometime link to or mirror Quake projects.

Personal websites are sometimes listed in modification readme files or linked to from Quake modification project websites, such as on the team webpage.

Start with the names and aliases you collected from the project website.

Search for each name together with terms such as `Quake`, `mod`, `mapping`, `programming` and the project name.

Investigate personal websites using the same approach as project websites: check their Wayback Machine captures, examine relevant pages and record any references, downloads or related projects you discover.

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

These gaps help identify releases that require further investigation, particularly those mentioned in announcements but absent from surviving download pages. Other historical sources may help establish whether these releases were publicly distributed and whether copies survive.

The next research chapters will help you investigate these questions using other historical sources.

## Record your discoveries

Add discoveries to the appropriate archival documents as you investigate each website:

| Discovery                              | Where to record it                                        |
| -------------------------------------- | --------------------------------------------------------- |
| Original project URL                   | `research/history.md`                                     |
| Archived website captures              | `research/history.md`                                     |
| Release announcements                  | Relevant release entry in `history.md`                    |
| Release dates and version numbers      | Relevant release entry in `history.md`                    |
| Original download URLs                 | Relevant release entry and `wishlist_urls.txt` if missing |
| Recovered files                        | `bin/` and the relevant release entry                     |
| Readmes and changelogs                 | Relevant release entry                                    |
| Developer websites                     | `research/history.md`                                     |
| Related projects                       | `research/notes.txt`                                      |
| Missing files and unresolved questions | `research/wishlist.txt` and `research/notes.txt`          |


Preserve important pages and downloadable evidence where possible, following the approach established earlier. A Wayback Machine URL is useful, but it should not be your only record of an important discovery. Archived pages and files can sometimes become inaccessible or behave differently over time.

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