---
title: 12. Search the Modern Web and Search Engines
weight: 50
---


# 12. Search the Modern Web and Search Engines

Many references to Quake modifications still survive on the modern web. Old websites have been copied, files have been mirrored, personal pages have been resurrected and historical discussions have been republished.

General-purpose search engines can help locate these resources using the information gathered during your earlier research.

Every discovery provides new search terms. A developer's name might lead to a personal website, while a recovered filename might reveal another copy of a missing release or a previously unknown distribution location.

## Search Multiple Search Engines

Different search engines use different indexes and ranking systems. A search that produces no useful results on Google may reveal valuable material on another engine.

Start with several general-purpose search engines:

- [Google](https://www.google.com/)\
    `https://www.google.com/`
- [Yandex](https://yandex.com/)\
    `https://yandex.com/`
- [DuckDuckGo](https://duckduckgo.com/)\
    `https://duckduckgo.com/`

Try important search terms across several engines rather than relying on a single set of results.

## Search the Modification and Related Names

Begin with the names recorded in `research/history.md` and `research/notes.txt`. Search the modification's official name, alternative spellings, abbreviations, earlier titles and development team names.

Also search for related project names, development teams and known aliases. A modification might have been renamed during development or distributed under a different name by a third-party website.

### Search developer names

Search developer names and aliases to locate personal websites, related projects and files distributed under different usernames.

Try combinations such as:

```
"Developer Name" Quake
"Developer Name" Action Quake
"developer_username" Quake mod
"developer_username" download
```

Results may reveal project pages, interviews, community profiles, old download directories and alternative mirrors.

Search for personal website domains and email addresses discovered in earlier research.

Treat identity matches carefully. A similar name or username does not automatically establish that two references concern the same person.

## Search Every Known Filename

By this stage, your research may have uncovered dozens or hundreds of filenames from historical announcements, Usenet discussions and recovered releases. Search engines provide another opportunity to locate references to these files or surviving copies.

Search each known archive filename, including alternatives discovered in historical references. Also search distinctive filenames found inside recovered releases.

Do not assume that a file is still available simply because you have found its name in an old announcement. Search engines might reveal another website hosting a copy, a file listing on a mirror or a reference to a different distribution location.

### Search exact filenames

Search filenames both with and without quotation marks. Quoted searches can reduce irrelevant results, while unquoted searches may reveal matches when punctuation or filename formatting differs.

Also try searching without quotation marks, particularly if the filename contains punctuation or if search engines interpret it differently.

Try variations when necessary:

```
"action15.zip"
action15.zip
"action_15.zip"
"actionquake15.zip"
```

### Search filenames inside recovered releases

Search distinctive filenames from inside recovered archives, including readmes, maps, configuration files and models.

For example:

```
"shadowarena_readme.txt"
"arena_final.bsp"
"shadow_player.mdl"
```

These searches can find copies of a release that were renamed or extracted before being distributed.

## Search Distinctive Readme Content

Search for distinctive phrases from recovered readmes, credits, installation instructions and changelogs.

For example, a fictional readme might contain:

```
Shadow Arena introduces a new team-based combat system
with custom weapons and modified player movement.
```

Search for a distinctive part of this text:

```
"new team-based combat system"
"modified player movement"
```

This can locate pages containing the readme even when the project name and original archive filename are absent.

Try shorter phrases if an exact search produces no results. The text may have been reformatted, copied with different punctuation or split across multiple lines.

## Search Known Historical URLs

Search historical URLs collected during earlier research. Even when the original destination is unavailable, other indexed pages may still reference it.

For example:

```
"http://example.com/quake/action/"
"ftp://ftp.example.com/pub/quake/action15.zip"
"example.com/~developer/actionquake"
```

This can reveal:

- Websites that linked to the original project.
- Mirror pages.
- Old directory listings.
- Forum discussions.
- Archived documentation.
- References to downloadable files.

Search domain names separately from complete URLs to discover other projects, directories and references associated with the same host.

### Search known mirrors and distribution locations

If you discover a mirror or download site, search for its name and domain alongside the modification name and known filenames.

For example:

```
"action15.zip" mirror
"Action Quake 2" downloads
"Action Quake 2" FTP
site:example.com "action15.zip"
```

The `site:` search operator restricts results to a particular domain. This is useful when you want to search a known website for a particular project or filename.

You can also search for known directory paths and filenames together.

These searches may reveal other copies of a release or additional files that were distributed alongside it.

## Explore Search Results Thoroughly

Explore beyond the first page of search results. Obscure personal homepages, fan sites and seemingly unrelated discussions may contain important historical references.

In particular:

- Open results that mention the project or its developers.
- Follow links to related websites.
- Inspect download pages and file listings.
- Follow links to other modifications and community resources.
- Look for references to old FTP servers.
- Investigate pages that appear to be personal archives.
- Search within promising websites for additional references.

When a result looks relevant, inspect the actual page. A search snippet can omit important information or display text from an unrelated part of the page.

### Follow links on relevant pages

Follow links from promising pages to other modifications, developer websites, download directories, FTP servers and historical community resources.

An old page with broken images and a basic HTML layout may contain more useful historical information than a polished modern website.

### Search within discovered websites

Use the `site:` operator to search promising websites for additional references to the modification, its developers and known filenames.

For example:

```
site:example.com "Action Quake 2"
site:example.com "action15.zip"
site:example.com "Developer Name"
```

This leads to an important limitation of general-purpose search engines.

## Understand What Search Engines Do Not Find

Search engines do not index the entire web. Historical websites, file archives and publicly accessible downloads may exist without appearing in search results.

### Some websites deliberately exclude themselves

Website owners can instruct search engines not to index their pages.

This can be done using mechanisms such as `robots.txt` and `noindex` directives.

A website might therefore be accessible to anyone who knows its address, while remaining absent from search results.

Some old websites that have been resurrected or copied may also retain exclusion settings from their original hosting environment.

Do not assume that a site does not exist simply because a search engine cannot find it.

### File archives are often not indexed

Publicly accessible file collections are not necessarily indexed. An Amazon S3 bucket, cloud storage account or unlinked web directory may contain thousands of ZIP files without providing crawlable webpages that search engines can discover.

This is especially relevant when investigating:

- Quake archives hosted on Amazon S3.
- Files stored on other cloud providers.
- Old FTP mirrors.
- Unlinked download directories.
- Personal backup collections.
- Large collections of ZIP files.
- Historical file repositories with limited web interfaces.

### Resurrected historical websites may not be indexed

Some historical websites, including old GeoCities pages and personal Quake sites, have been reconstructed on modern domains. These collections may contain original readmes, download links and project histories.

However, search engines may not index them because they have few incoming links, retain restrictive indexing settings or were only recently published. If you discover such a collection through a forum or archive catalogue, explore it directly.

### Manually explore discovered websites

When you discover a relevant website, browse its navigation, project indexes, download directories, sitemap files and links to other archives. These may reveal pages and files absent from search results.

A site might have an index page listing dozens of modifications, while individual project pages are not indexed at all.

You may need to browse the site and follow its internal links to discover the relevant content.

If you find a directory listing, inspect its files and subdirectories. A page containing only a list of ZIP files might be exactly what you need.

## Investigate Unindexed File Collections

When you discover an FTP server, file mirror or download directory, investigate it directly rather than relying on search results. A collection may contain files that search engines have never indexed.

The next chapter explains how to explore these historical file collections.

## Build a Systematic Search Process

By this stage, you should have accumulated a substantial collection of search terms, including project names, developer aliases, release filenames, distinctive readme content, historical URLs and known mirrors.

Organise these terms into a search checklist in `research/notes.txt` or a separate document

For each important search term, try multiple search engines and record useful discoveries.

For example:

| Search term    | Google   | Yandex   | DuckDuckGo | Result             |
| -------------- | -------- | -------- | ---------- | ------------------ |
| Action Quake 2 | Searched | Searched | Searched   | Project references |
| action15.zip   | Searched | Searched | Searched   | Possible mirror    |
| Developer Name | Searched | Searched | Searched   | Personal website   |
| aq2_readme.txt | Searched | Searched | Searched   | CD listing         |

The table is illustrative. You do not need to record every unsuccessful search. The goal is to make sure important terms are not forgotten and that you do not repeatedly perform the same searches without making progress.

### Add new discoveries to your search terms

Research should be iterative.

Each discovery can reveal additional search terms. A developer's website might identify an unknown release, its filename might lead to a mirror, and that mirror might reveal related projects worth investigating.

Repeat your searches as new information becomes available rather than treating web searching as a one-time activity.

### Record useful discoveries

Record useful search results in the appropriate archival documents, including release evidence in `history.md`, research leads in `notes.txt`, and missing files or historical URLs in the wishlist files.

## Summary

Modern search engines provide another way to discover historical Quake websites, surviving files and references that escaped earlier research.

Search across multiple engines using project names, developer aliases, filenames, readme content and historical URLs. Follow promising results and investigate their associated websites.

Remember that many historical collections are not indexed. Search engines are useful discovery tools, but direct investigation of websites, FTP servers and file archives remains essential.

**Outcome:** You can systematically search the modern web using information accumulated during earlier research.

In the next chapter, we will investigate FTP archives and old download directories. These are particularly important because many historical Quake modifications were distributed directly through FTP servers, often without an associated webpage that a modern search engine could discover.