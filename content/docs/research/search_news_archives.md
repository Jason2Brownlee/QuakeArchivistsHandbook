---
title: 9. Research Gaming News Archives
weight: 20
---

# 9. Research Gaming News Archives

In the previous chapter, you learned how to investigate original project websites and use the Wayback Machine to reconstruct their public-facing history.

Your next source of information is contemporary gaming news websites.

During the late 1990s and early 2000s, several websites regularly reported on Quake modifications, new releases, community projects and developments in PC gaming. These sites often linked directly to project homepages and download locations. They also reported on new versions, patches, reviews, previews and other events that might not have been documented on the original project website.

This makes gaming news archives particularly valuable for historical research.

A project homepage might have disappeared, or its news section might contain only a few surviving announcements. A gaming news website could have reported on the same release, preserved the original download links and provided additional information about where the files were hosted.

In some cases, a news article may be the only surviving evidence that a particular release existed.

This chapter explains how to find and investigate contemporary gaming news websites, search their archives and connect their reports to the releases in your historical record.

## Identify relevant gaming news websites

Start by identifying gaming news websites that were active during the period when the modification was developed.

Some particularly useful sources for Quake-related research include:

- **PlanetQuake** (`planetquake.com`): A major Quake community site with project pages, news and links to modifications.
- **Telefragged** (`telefragged.com`): A Quake-focused website that covered community projects and related news.
- **Blue's News** (`bluesnews.com`): A long-running PC gaming news site that reported on Quake modifications, patches, downloads and other gaming developments.
- **Redwoods News** (`redwood.stomped.com`): A historical gaming news source with coverage of Quake and its community.
- **Shacknews** (`shacknews.com`), formerly Shugashack: A PC gaming news site that covered games, modifications and community developments.

There were also many smaller Quake news sites, personal news pages and general PC gaming websites that occasionally reported on modifications.

Do not restrict your research to the largest or best-known sites. A small community news page might contain the only surviving announcement for an obscure modification.

You can discover additional news sites through links from:

- Original project websites.
- Developer personal websites.
- Other Quake community sites.
- Contemporary gaming news articles.
- Historical link directories.

Record relevant websites and their URLs in your research notes. You can investigate each one using the same general approach as the original project websites in Chapter 4.

## Find archived versions of gaming news websites

Many historical gaming news websites have changed their design, moved to new domains or disappeared entirely. The Internet Archive's Wayback Machine (`https://web.archive.org`) is therefore an important starting point.

Enter the news website's original domain and inspect its capture history.

For example:

```
http://www.bluesnews.com/
http://www.planetquake.com/
http://www.telefragged.com/
```

Look for captures from the period when your target modification was active.

There are two particularly useful types of archived pages to investigate:

1. The main news page, often called `index.html` or simply the homepage.
2. Dedicated news archive pages containing older articles.

You should examine both.

### Inspect archived main news pages

The main news page is often the easiest place to start.

It may contain a list of recent headlines, each linking to a full article or story.

If you know approximately when a release was announced, inspect captures from around that date.

For example, suppose your research indicates that a modification's version 1.0 release was announced in August 1999.

Start by examining archived captures from August 1999. Look through the headlines and follow anything that might relate to the modification.

You might find an announcement that includes the project name, a download link or a reference to the original homepage.

If the archived main page is incomplete, try captures from nearby dates. A story might appear in one capture but not another.

### Inspect dedicated news archives

Many news websites maintained separate archive pages containing older stories.

These archives are often more useful than the main news page because they preserve a much larger portion of the site's history.

Look for links or paths containing terms such as:

```
archive
archives
news
oldnews
1998
1999
```

For example, a website might have pages structured like:

```
/news/1998/index.html
/news/1999/index.html
/archives/1998.html
/archives/1999.html
```

These are illustrative paths. The actual structure will vary between websites.

Use the Wayback Machine to inspect these URLs individually. An archive page may have been captured even if the corresponding main news page was not.

You can also use the CDX interface described in Chapter 4 to discover archived URLs beneath a news site's domain.

The important point is to investigate both the front page and the site's historical archives. A main page capture might be missing an article that survives in a dedicated archive, or an archive page might be incomplete while the original headline remains visible on an older main page.

Here are three archived major Quake news pages I frequent often (via the Wayback Machine):

* BluesNews circa July 1996 to Feb 1999\
  `https://www.bluesnews.com/archives/`
* Redwood's 3D News (later Stomped) circa April 1996 to April 1999\
  `http://redwood.stomped.com/archives.html`
* ShugaShack (later ShackNews) circa March 1997 to Jun 1999\
  `http://shugashack.com/archives/archives.htm`


## Search news pages for the modification's name

Once you have located an archived news page, search its contents for the modification's name.

The simplest technique is to use your browser's built-in Find function.

Press:

- `Ctrl + F` on Windows or Linux.
- `Command + F` on macOS.

Enter the modification's name or a distinctive part of it.

For example, if you are researching Action Quake, search for:

```
Action Quake
```

Also try variations:

```
ActionQuake2
AQ2
Action Quake 2
Action Quake2
Action
```

A modification might be referred to by a shortened name, an acronym or a slightly different title.

Search for developer names as well. A news site might report on a release under the developer's name rather than the project's name.

If the page contains many stories, searching can quickly identify relevant headlines. Open each promising result and examine the full article.

Do not rely exclusively on the browser's Find function. It can only search the content currently loaded in the page. Some news archives split stories across multiple pages, use separate article pages or contain links to external content.

You may need to inspect several pages or follow links manually.

### Search the entire active period of the project

Do not limit your investigation to the dates of known releases.

If a modification was active from 1997 to 2000, search news archives throughout that period.

You might discover:

- An early announcement of the project.
- A public beta that was not documented on the project homepage.
- A major release.
- A patch or update.
- A new map pack.
- A mirror announcement.
- A review or preview.
- A development milestone.
- The announcement that development had ended.

This is particularly important when the original project website has an incomplete news section or has disappeared entirely.

A gaming news website may have reported on releases that are no longer mentioned anywhere on the surviving project homepage.

## Use known release dates to guide your search

One of the most effective techniques is to use dates you have already discovered during your research.

Suppose you have established from an archived project homepage that version 1.0 was released in August 1999.

You now have a specific period to investigate.

Inspect archived news pages from:

- The weeks immediately before the release.
- The week of the release.
- The weeks immediately after the release.

Why search before the release? A news site might publish a preview or announcement before the files become available.

Why search afterwards? A news site might report the release several days later, or publish a follow-up story when mirrors become available. This is very common in my experience.

For a release in August 1999, you might examine captures from late July, August and early September.

If you find a relevant article, record its publication date and compare it with the date already recorded in `history.md`.

The dates might differ. For example:

- The file timestamp in the .zip archive is 08 August.
- The developer announces the release on 10 August.
- A gaming news site reports it on 12 August.
- A mirror becomes available on 15 August.
- A magazine CD containing the release is published in October.

These are five separate historical events. Together, they provide a more complete picture of the release and its distribution.

The release was created and perhaps tested locally before being uploaded to a public facing server. The differing dates allow corroborating evidence that version was real and release occurred. The public release date is probably taken as the developers announcement.

### Search around every known release

Repeat this process for every release you have identified.

For example, suppose your current release record contains:

| Release     | Known date     |
| ----------- | -------------- |
| Public beta | March 1998     |
| Version 0.5 | September 1998 |
| Version 1.0 | February 1999  |
| Version 1.1 | August 1999    |

Use these dates to guide your searches across the relevant news websites.

You may find that one site reported the beta, another covered version 1.0, and a third announced a mirror for version 1.1.

This is useful because no single news website is likely to have covered every release.

It also works in reverse. If you find an article announcing a version that is not in your release record, you have discovered a new research lead.

Add it to the `Releases and Chronology` section of `history.md`, even if the file itself has not yet been recovered.

## Investigate individual news articles

When you find a relevant news announcement, carefully examine its contents.

A short headline might not reveal much, but the article itself can contain several useful links and details.

Look for:

- The release name or version number.
- The announcement or publication date.
- The developer or project name.
- A link to the original project homepage.
- A direct download link.
- Links to alternative mirrors.
- References to related projects.
- A description of new features or changes.
- Comments about availability or distribution problems.

A news article might provide the missing link between a release and its original homepage or download location.

For example, you might have found a reference to version 0.95 in a forum discussion, but you do not know where it was originally distributed.

A contemporary news article could identify the release, link to the developer's homepage and provide two alternative download locations.

That one article could resolve several outstanding questions.

### Follow every relevant link

Do not simply read the article and move on.

Follow the links associated with the modification.

A news story might link to:

1. The original project homepage.
2. A developer's personal website.
3. The main download location.
4. One or more mirrors.
5. A review or earlier announcement.

Record these URLs exactly as they appear.

If a link points to another website, investigate that website using the Wayback Machine. If it points to a file, check whether the file itself was archived or whether it might survive elsewhere.

An article can therefore become the starting point for another round of research.

### Look for stories about mirrors

Mirror announcements deserve particular attention.

A news site might report that a popular modification is difficult to download because the original server is unavailable or overloaded.

The article may provide alternative download links, sometimes hosted directly by the news website.

These links can be extremely valuable when the original project website no longer exists.

They might also reveal files that were distributed under filenames different from those used by the developer.

Record each mirror separately. A news site's copy may be an important source for recovering a release, even if it was not the original distribution location.

## Preserve news announcements in the release record

When you discover a relevant article, add it to the appropriate release entry in `research/history.md`.

Do not simply save a browser bookmark or add the article to a general list of references. The important information should be connected directly to the release it describes.

I recommend preserving a short quotation from the announcement, along with the article URL, archived URL and any links to the modification.

For example:

```
#### Version 0.95

Mentioned on Blue's News:

* Original article:
  https://www.bluesnews.com/s/234326/action-quake-mirror

* Archived article:
  [Wayback Machine URL]

* Publication date:
  15 August 1998, 6:13 pm ET

Announcement excerpt:

> The new Action Quake2 has been tough to come by
> since none of the mirrors are up yet.

Links in news:

* ftp://ftp.gamesnet.net/pub/bluesnews/quake2/action/actn95cl.exe
* ftp://ftp.gamesnet.net/pub/bluesnews/quake2/action/actn95cl.zip

Information established:

- Version: 0.95
- Two downloadable files were available.
- Blue's News provided alternative copies.
- The original mirrors were reportedly unavailable.
```

The example is based on the type of information found in historical news reporting. The excerpt is illustrative.

This format preserves the most useful parts of the article without requiring you to copy the entire story into your historical record.

The original article and archived page provide the supporting evidence. The quotation reminds you what the article said, while the links allow you or another researcher to investigate the original material.

### Record the full download links

Pay particular attention to links included in news stories.

Preserve the complete URL, including:

- The protocol, such as `http` or `ftp`.
- The hostname.
- The directory path.
- The filename.
- Any query parameters, if present.

For example:

```
ftp://ftp.gamesnet.net/pub/bluesnews/quake2/action/actn95cl.zip
```

Do not shorten the URL or replace it with a modern equivalent.

The original location might no longer work, but it can still help you identify the file and search for copies elsewhere.

If the article links to multiple files, record each one separately. A story might provide an installer, a ZIP archive, a patch or a server-only version.

These could represent different distributions of the same release.

## Use news articles to discover missing releases

One of the most valuable uses of gaming news archives is discovering releases that are missing from your existing research.

Suppose the original project homepage has only two surviving announcements:

- Version 1.0, released in April 1998.
- Version 1.2, released in November 1998.

You search Blue's News and find an article from August 1998 announcing version 1.1.

This is a new discovery.

You should:

1. Add the filename and release date to `README.md`
2. Add version 1.1 to `research/history.md`.
3. Record the announcement date and any release date supported by the article.
4. Record the filenames and download URLs.
5. Add any unrecovered files to `research/wishlist.txt`.
6. Add the original download URLs to `research/wishlist_urls.txt`.

You now have a more complete release sequence.

This is particularly important when the original project website did not have a complete news section, or when its archived captures are missing.

A gaming news website may have preserved announcements that the developers' own website no longer contains.

### Look for releases mentioned indirectly

Not every article will explicitly announce a new version.

A story might say:

- "The latest version of the modification is now available."
- "An updated client has been released."
- "A new map pack has been added."
- "The developers have uploaded a new server package."
- "The project has received a major update."

These references may indicate a new release or a supplementary distribution.

Record what the article actually establishes. Do not automatically assign a version number if none is provided.

For example:

```
#### Unidentified update

- Date: August 1999
- Version: Unknown
- Filename: Unknown
- Status: Unverified
- Evidence:
  Blue's News reports that an updated client
  is available.
- Questions:
  - Is this a new version or a patch?
  - Can the original download be identified?
```

You can investigate the announcement further using the links and other references it provides.

## Search beyond the major news websites

The websites listed at the beginning of this chapter are useful starting points, but they are not the only sources worth investigating.

Many smaller websites reported on Quake modifications. Some were dedicated to Quake, while others covered PC gaming more generally.

You might discover these sites through links in articles, original project homepages or other community websites.

Also consider searching for:

- Quake news sites.
- Quake II and Quake III news sites.
- PC gaming news archives.
- Gaming magazine websites.
- Mod download directories.
- Individual community news pages.

A smaller site might have covered a modification that the larger news sites ignored. This is especially true for larger modifications that have their own dedicated sub-community like Team Fortress and Capture The Flag.

You can also search the web for distinctive phrases from an announcement, filenames or developer names. Sometimes a story has been reproduced or referenced by another website.

Treat these discoveries as additional evidence and record the original source wherever possible.

## Chapter summary

Contemporary gaming news websites provide an independent source of historical information about Quake modifications.

They can help establish release dates, identify missing versions, locate original project websites and discover download mirrors that are no longer mentioned elsewhere.

The main ideas from this chapter are:

- Search contemporary Quake and PC gaming news websites, including PlanetQuake, Telefragged, Blue's News, Redwoods News and Shacknews.
- Use the Wayback Machine to inspect archived main news pages and dedicated news archives.
- Search individual pages using the browser's Find function.
- Use known release dates to guide searches around the likely announcement period.
- Search the entire period during which the modification was active.
- Examine individual articles and follow their links to project websites, downloads and mirrors.
- Use news reporting to discover releases missing from the original project website.
- Preserve relevant announcement excerpts, publication dates, original URLs and archived page links in `history.md`.

**Outcome:** You can use contemporary gaming news reporting to discover additional releases, websites, developers and historical download locations. You can also use news articles as supporting evidence to reconstruct a project's release history, particularly when the original project website is incomplete or no longer available.

In the next chapter, you will investigate Usenet archives. These can preserve discussions between developers and players, release announcements, technical support questions and references to files that may not appear in either the original project website or gaming news archives.
