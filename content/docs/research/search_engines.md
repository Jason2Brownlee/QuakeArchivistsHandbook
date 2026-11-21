---
title: 12. Search the Modern Web and Search Engines
weight: 50
---


# 12. Search the Modern Web and Search Engines

In the previous chapters, we investigated historical project websites, gaming news archives, Usenet discussions and physical media. These sources provide valuable evidence, but they are only part of the picture.

Many references to Quake modifications still exist somewhere on the modern web. Old websites have been copied, personal pages have been resurrected, files have been mirrored and historical discussions have been republished. General-purpose search engines can help locate these surviving resources.

This chapter explains how to use search engines systematically, using the information accumulated during your earlier research.

The key idea is that every discovery gives you new search terms. A project name leads to a developer name. A developer name leads to a personal website. A recovered release reveals filenames. Those filenames can lead to other copies of the same release or previously unknown distribution locations.

## Search Multiple Search Engines

Do not rely exclusively on Google.

Different search engines maintain different indexes of the web. They use different crawling systems, ranking algorithms and approaches to indexing pages. Consequently, a search that produces no useful results on one search engine might produce valuable results on another.

Start with several general-purpose search engines:

- [Google](https://www.google.com/)\
    `https://www.google.com/`
- [Yandex](https://yandex.com/)\
    `https://yandex.com/`
- [DuckDuckGo](https://duckduckgo.com/)\
    `https://duckduckgo.com/`

You can also try other search engines that are available at the time of your research.

The goal is not to find one perfect search engine. It is to search across several independent indexes and compare what they return.

For each important search term, try more than one search engine. This is particularly important when researching older material, where a single indexed page might be the only surviving reference to a modification or download.

## Search the Modification and Related Names

Begin with the information already collected in `research/history.md` and `research/notes.txt`.

Try searching for the modification's name, including alternative spellings and naming conventions.

For example, a project might be referred to as:

```
Action Quake 2
Action Quake II
ActionQuake2
AQ2
Action Quake
```

Search each variation separately.

Also search for related project names, development teams and known aliases. A modification might have been renamed during development or distributed under a different name by a third-party website.

Do not assume that the name used in the original project website is the only name that appears elsewhere.

### Search developer names

Search for the names and usernames of developers associated with the modification.

A developer might have maintained a personal website, contributed to another project or posted files under a username that differs from their real name.

Try combinations such as:

```
"Developer Name" Quake
"Developer Name" Action Quake
"developer_username" Quake mod
"developer_username" download
```

Search for personal website domains and email addresses discovered in earlier research.

These searches can uncover:

- Personal project pages.
- Social media pages.
- Other modifications by the same developer.
- Old download directories.
- Development team websites.
- Interviews and community profiles.
- Links to mirrors and related projects.

Treat identity matches carefully. A similar name or username does not automatically establish that two references concern the same person.

## Search Every Known Filename

Filename searching becomes increasingly valuable as your research progresses.

At the beginning of an archive project, you might know only the name of the modification. After researching websites, news articles, Usenet messages and CD collections, you may have identified dozens or hundreds of filenames associated with it.

Each filename becomes another search term.

For example, you might have collected the following filenames:

```
action15.zip
actionquake15.zip
aq2-1.5.zip
aq2_readme.txt
action_config.cfg
teamplay_guide.txt
```

Search for each one.

Do not assume that a file is still available simply because you have found its name in an old announcement. Search engines might reveal another website hosting a copy, a file listing on a mirror or a reference to a different distribution location.

### Search exact filenames

Use quotation marks to search for an exact filename:

```
"action15.zip"
```

This can reduce irrelevant results and help locate pages that mention the specific file.

Also try searching without quotation marks, particularly if the filename contains punctuation or if search engines interpret it differently.

Try variations when necessary:

```
"action15.zip"
action15.zip
"action_15.zip"
"actionquake15.zip"
```

Search for both the original archive filename and any alternative names discovered during your research.

### Search filenames inside recovered releases

Do not restrict your searches to the names of ZIP archives.

Inspect recovered releases and identify distinctive filenames within them. Search for readmes, maps, configuration files, models and other custom assets.

For example:

```
"shadowarena_readme.txt"
"arena_final.bsp"
"shadow_player.mdl"
```

These searches can find copies of a release that were renamed or extracted before being distributed.

This is particularly useful when a website or CD collection contains the modification under a generic filename or directory.

As your archive grows, maintain a list of known filenames and use it as a regular source of search terms.

## Search Distinctive Readme Content

A readme file often contains information that is much easier to search for than the modification's name.

Look for distinctive sentences, descriptions, credits, installation instructions and copyright notices.

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

Other useful search terms include:

- Developer names and email addresses.
- Distinctive phrases from the introduction.
- Unusual installation instructions.
- Copyright statements.
- Changelog entries.
- Credits and acknowledgements.
- Names of custom maps and assets.

Try shorter phrases if an exact search produces no results. The text may have been reformatted, copied with different punctuation or split across multiple lines.

A particularly useful approach is to search for a phrase that is unlikely to appear in unrelated Quake modifications.

## Search Known Historical URLs

During earlier research, you will have collected original URLs from project websites, news articles, Usenet messages and CD documentation.

Search for these URLs directly.

For example:

```
"http://example.com/quake/action/"
"ftp://ftp.example.com/pub/quake/action15.zip"
"example.com/~developer/actionquake"
```

A search engine might have indexed a page containing the old URL even though the original website is no longer available.

This can reveal:

- Websites that linked to the original project.
- Mirror pages.
- Old directory listings.
- Forum discussions.
- Archived documentation.
- References to downloadable files.

Also search for just the domain name, without the full path.

A domain might have been used for several different projects or distribution directories. Searching for it can reveal pages that you would not find using the original project URL alone.

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

Do not stop after looking at the first page of search results.

Historical research often produces unusual results. An old personal homepage, an obscure fan site, a small file archive or a seemingly unrelated discussion might contain exactly the information you need.

Read the search results carefully and investigate promising links.

In particular:

- Open results that mention the project or its developers.
- Follow links to related websites.
- Inspect download pages and file listings.
- Follow links to other modifications and community resources.
- Look for references to old FTP servers.
- Investigate pages that appear to be personal archives.
- Search within promising websites for additional references.

Continue through the search result pages rather than stopping at the first few results.

When a result looks relevant, inspect the actual page. A search snippet can omit important information or display text from an unrelated part of the page.

### Follow links on relevant pages

A useful page can lead to many more discoveries.

For example, an old Quake fan site might contain:

- A list of recommended modifications.
- Links to developers' personal websites.
- A download directory.
- A list of related projects.
- Links to other Quake websites.
- A collection of old FTP addresses.

Follow these links, even when the destination looks outdated or unfamiliar.

An old-looking page with broken images and a basic HTML layout might be more valuable to your research than a modern website with polished presentation.

Do not judge a source by its appearance.

### Search within discovered websites

When you find a promising website, investigate it beyond the page returned by the search engine.

Search for the modification name, developer name and known filenames in combination with the website's domain.

For example:

```
site:example.com "Action Quake 2"
site:example.com "action15.zip"
site:example.com "Developer Name"
```

Also inspect the website's navigation, index pages, directory listings and links to related sections.

A website might contain an entire archive of old Quake modifications even though the search engine has indexed only its homepage.

This leads to an important limitation of general-purpose search engines.

## Understand What Search Engines Do Not Find

Search engines are useful, but they do not contain a complete index of the web.

Many current websites, file archives and historical collections are not indexed. A page can exist and be publicly accessible without appearing in Google, Bing or any other search engine.

This is particularly important when researching old Quake material.

### Different search engines have different indexes

As discussed earlier, search engines do not necessarily index the same pages.

A page missing from Google's results might appear in Yandex or DuckDuckGo. Another search engine might have indexed a different version of the page or retained a reference that is no longer prominent elsewhere.

This is one reason to search multiple engines throughout your research rather than treating one search engine as authoritative.

### Some websites deliberately exclude themselves

Website owners can instruct search engines not to index their pages.

This can be done using mechanisms such as `robots.txt` and `noindex` directives.

A website might therefore be accessible to anyone who knows its address, while remaining absent from search results.

Some old websites that have been resurrected or copied may also retain exclusion settings from their original hosting environment.

Do not assume that a site does not exist simply because a search engine cannot find it.

### File archives are often not indexed

Many file archives are difficult for general search engines to discover.

For example, a collection of Quake modifications might be stored in an Amazon S3 bucket or another cloud storage service.

The files might be publicly accessible, but the storage location may not provide ordinary webpages for search engines to crawl.

Similarly, a web server might contain thousands of ZIP files in directories that are not linked from an indexed homepage.

A search engine cannot reliably discover every file in such a collection.

This is especially relevant when investigating:

- Quake archives hosted on Amazon S3.
- Files stored on other cloud providers.
- Old FTP mirrors.
- Unlinked download directories.
- Personal backup collections.
- Large collections of ZIP files.
- Historical file repositories with limited web interfaces.

### Resurrected historical websites may not be indexed

Some old websites have been brought back online using copied files or preserved website content.

For example, old GeoCities websites and personal Quake pages may have been reconstructed and hosted on modern domains.

These sites can contain valuable material, including old download links, readmes and project histories.

However, their pages may not be indexed by search engines. This might be because the site is relatively new, its pages are not linked from elsewhere or it deliberately excludes itself from indexing.

You might discover a resurrected website through a forum post, an archive catalogue or a link on another historical site. Once you find it, investigate it directly.

Do not rely on search engines to discover every page within it.

### Manually explore discovered websites

When you find a relevant website, explore its structure manually.

Look for:

- Homepage links.
- Navigation menus.
- Project indexes.
- Download sections.
- File directories.
- Links to other websites.
- Sitemap files.
- Directory listings.
- Older versions of pages.
- References to other archive locations.

A site might have an index page listing dozens of modifications, while individual project pages are not indexed at all.

You may need to browse the site and follow its internal links to discover the relevant content.

If you find a directory listing, inspect its files and subdirectories. A page containing only a list of ZIP files might be exactly what you need.

The important principle is that search engines are discovery tools, not complete catalogues of the web.

## Know the Limitations of Searching for Files

General-purpose search engines are not necessarily good at finding files on old FTP servers or obscure web directories.

An FTP server might contain hundreds of useful files, but if there are no indexed webpages linking to them, a search engine may never discover them.

Similarly, a web server might have a directory containing:

```
/pub/quake/mods/
    action15.zip
    arena2.zip
    bots.zip
    maps.zip
```

The files might be accessible if you know the directory URL, but the search engine might not have indexed either the directory listing or the individual files.

This means that searching for a filename is not guaranteed to find every surviving copy.

You should still search for filenames because it is a valuable technique, but recognise that a lack of results does not establish that a file is unavailable.

When you discover an old FTP server, mirror or obscure directory, investigate it directly. This is the subject of the next chapter.

## Build a Systematic Search Process

By this stage of your research, you should have accumulated a substantial collection of information:

- Modification names and alternative spellings.
- Developer names and usernames.
- Development team names.
- Release versions.
- Original archive filenames.
- Filenames found inside recovered releases.
- Distinctive readme phrases.
- Project website domains.
- Historical download URLs.
- Known mirror names and domains.
- Related projects and community websites.

Use this information as a structured collection of search terms.

A simple approach is to maintain a search checklist in `research/notes.txt` or a separate file if your project has become large enough to justify one.

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

For example:

1. You search for the modification name and discover a developer's personal website.
2. You inspect the website and find a new version number.
3. You search for the version number and discover an alternative filename.
4. You search for the filename and find a mirror.
5. The mirror reveals another modification by the same developer.
6. You search for that related project and discover another website.

Each discovery creates new opportunities for searching.

Do not treat the search process as something that happens once at the beginning of the project. Return to it whenever you uncover new information.

### Record useful discoveries

Update your existing research documents as you find information.

- Add new release evidence to `research/history.md`.
- Record informal leads and questions in `research/notes.txt`.
- Add missing files to `research/wishlist.txt`.
- Add unrecovered download locations to `research/wishlist_urls.txt`.

This keeps your search process connected to the archival record rather than allowing useful discoveries to disappear into browser history.

## Summary

General-purpose search engines can reveal surviving references and copies of historical Quake modifications that have not been found through the earlier research methods.

Search Google, Yandex, DuckDuckGo and other available engines because their indexes differ. Search project names, developer names, filenames, readme content, historical URLs and known distribution locations.

As your research progresses, filename searching becomes increasingly valuable. Every recovered release provides additional filenames and distinctive content that can be used to locate other copies.

However, remember that search engines do not index the entire web. Many file archives, cloud storage collections, FTP servers and resurrected historical websites are not discoverable through ordinary search results. When you find a relevant website, explore it manually rather than relying on its indexed pages alone.

**Outcome:** You can systematically search the modern web using information accumulated during earlier research.

In the next chapter, we will investigate FTP archives and old download directories. These are particularly important because many historical Quake modifications were distributed directly through FTP servers, often without an associated webpage that a modern search engine could discover.