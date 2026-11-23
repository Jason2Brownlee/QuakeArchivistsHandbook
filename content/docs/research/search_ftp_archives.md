---
title: 13. Search FTP Archives and File Indexes
weight: 60
---

# 13. Search FTP Archives and File Indexes

FTP archives were among the most important distribution channels for Quake modifications during the 1990s. Developers and community members uploaded maps, patches, utilities and modifications to FTP servers, where they were often copied to mirrors around the world.

Although many original servers have disappeared, portions of their collections survive in modern mirrors and historical archives.

This chapter explains how to locate these collections, search their contents and investigate the original distribution locations of recovered files.


## Understand Historical FTP Archives

FTP (File Transfer Protocol) allowed users to upload and download files from remote servers. Quake communities relied heavily on these servers, with releases distributed through central archives, community hosting services and networks of mirrors.

Several important historical archives became well-known distribution locations:

- **idgames2** was a major archive of files for Quake-engine games. It included Quake maps, modifications, utilities and other content. Initially hosted on `cdrom.com` and later `gamers.org`.
- **PlanetQuake** was a major Quake community website and hosting service. It hosted individual modification websites and maintained an FTP archive of their files.
- **Telefragged** was another Quake community website and hosting service, with downloadable modifications and related material.
- **Games Domain** was a general PC gaming website that also maintained downloadable game files.

These services organised files differently. PlanetQuake and Telefragged hosted individual community projects, while `idgames2` operated primarily as a central file archive. Their directory structures reflect these differences, as we will examine below.

Finding a file in one of these archives establishes a distribution location, but does not necessarily identify where the release originated.

## Start with Modern Mirrors of Historical Archives

Several modern services preserve historical FTP directory trees and their downloadable files:

**Gamers.org mirrors**

Gamers.org hosts mirrors of several historical gaming FTP archives, such as:

- [id Software FTP archive](https://www.gamers.org/pub/mirrors/ftp.idsoftware.com/)\
	`https://www.gamers.org/pub/mirrors/ftp.idsoftware.com/`
- [PlanetQuake FTP archive](https://www.gamers.org/pub/mirrors/ftp.planetquake.com/)\
	`https://www.gamers.org/pub/mirrors/ftp.planetquake.com/`
- [Games Domain FTP archive](https://www.gamers.org/pub/mirrors/ftp.gamesdomain.co.uk/)\
	`https://www.gamers.org/pub/mirrors/ftp.gamesdomain.co.uk/`
- [idgames2 archive](https://www.gamers.org/pub/idgames2/)\
	`https://www.gamers.org/pub/idgames2/`

The Gamers.org `idgames2/` directory for Quake and related games was and is currently mirrored in many places, such as:

- ftp://ftp.fu-berlin.de/pc/games/idgames2/
- https://ftp.fu-berlin.de/pc/games/idgames2/
- https://www.quaddicted.com/files/idgames2/
- https://ftpmirror1.infania.net/pub/idgames2/
- https://mirror.braindrainlan.nu/pub/idgames2/
- https://files.xvertigox.com/idgames2/

Some of these mirrors are more or less reliable than others, and some may disappear by the time you read this.

For more information on mirrors see:

- [Gamers.org Community Archives](https://www.gamers.org/ftp/archives.html)\
	`https://www.gamers.org/ftp/archives.html`

**Dukeworld**

Dukeworld preserves files from several historical gaming archives, including a PlanetQuake and Telefragged mirrors.

- [Dukeworld Downloads](https://dukeworld.com/)\
	`https://dukeworld.com/`

Specifically:

- https://dukeworld.com/idgames2/
- https://dukeworld.com/planetquake/
- https://dukeworld.com/telefragged/

**Quaddicted**

Quaddicted maintains a large collection of Quake files, including modifications, maps and other content. Its file archive and associated mirrors are particularly useful when researching Quake 1.

- [Quaddicted Files](https://www.quaddicted.com/files/)\
	`https://www.quaddicted.com/files/`

The Quaddicted file archive is large and is being added to in an ad hoc manner.

### Understand how the archives organise their files

Different archives used different approaches to organising their contents. Understanding these arrangements makes it easier to find files and reconstruct the distribution history of a modification.

**PlanetQuake and Telefragged organised files around hosted projects.**

PlanetQuake and Telefragged often organised their FTP directories around hosted projects. A project's directory might contain releases, patches, maps, documentation, screenshots and website resources.

Inspect the entire directory to identify supplementary files and versions that may not appear in surviving announcements.

**idgames2 organised files by game and content category.**

Rather than organising everything around hosted project websites, idgames2 generally categorised files by content type, game or modification category. You will encounter directories for maps, QuakeC modifications, utilities and other types of content.

Some useful locations in the modern Gamers.org archive include:

- [Quake 1 QuakeC modifications](https://www.gamers.org/pub/idgames2/quakec/)\
	`https://www.gamers.org/pub/idgames2/quakec/`
- [Quake 2 files](https://www.gamers.org/pub/idgames2/quake2/)\
	`https://www.gamers.org/pub/idgames2/quake2/`

This means that searching idgames2 often requires looking in the appropriate category rather than searching for a project-specific directory.

**Use the archive structure to guide your search.**

Whichever archive you investigate, examine neighbouring directories and subdirectories for related releases, patches and documentation.

Do not assume that every mirror is complete or that its contents are identical to the original server. Different mirrors may have been created at different times, may contain different subsets of files, or may have been updated independently.

## Search FTP File Indexes

FTP file indexes can help locate alternative copies of known releases and discover previously unidentified files. Two useful services are:

- [FileMood](https://filemood.com/)\
	`https://filemood.com/`
- [Mamont's Open FTP Index](https://www.mmnt.net/)\
	`https://www.mmnt.net/`

Search engines of this kind can help discover files across multiple FTP servers and indexed directories. Their coverage varies, and they may not include every historical archive.

Search original release filenames, known variations, patches and distinctive files found inside recovered archives. Project and development team names may also produce useful matches.

For example, if earlier research identified `actionq2.zip`, search for that exact filename. Then try related forms such as `actionq2`, `actionq2_1.5.zip`, or distinctive filenames found inside the archive.

Filename searches may uncover mirrors that do not mention the project's name or reveal previously unknown versions. For example, finding `actionq2_1.6.zip` when only versions 1.4 and 1.5 are documented provides a lead worth investigating. Verify the file's contents before adding the release to your historical record.

### Accessing FTP Servers

Some FTP search engines provide links directly to the FTP server and directory containing a matching file. You may need an FTP client to browse these locations or download the files.

Modern web browsers generally no longer support direct FTP access, so a dedicated FTP client is often required. One popular open-source option is [FileZilla](https://filezilla-project.org/) (`https://filezilla-project.org/`).

When connecting to a public FTP server, try anonymous access. Typical connection details are:

- **Host:** The FTP server hostname from the search result.
- **Username:** `anonymous`
- **Password:** Your email address.

Some servers accept any password for anonymous access, while others may require an email address or another value. Follow any instructions provided by the server.

Once connected, browse the directories and inspect or download relevant files. Verify search results against the actual server where possible, since FTP indexes may be incomplete or outdated.

## Inspect FTP Directory Structures

FTP directory listings can reveal which files were available, how they were organised and which versions were distributed together. Archives may group material by game, project, developer or content category, providing clues about additional releases and related files.

When you locate a relevant directory, inspect its parent directory and neighbouring directories as well. A modification may have been stored in a general `mods/` directory, while related patches or documentation were placed elsewhere.

Some FTP archives also contain special index files, upload summaries and historical directory listings that can reveal additional information about their contents. We will investigate these resources in Chapter 21, Advanced Research Tips.

Also inspect directory listings for files that you have not yet identified. A release might have a different filename from the one mentioned in a news article, or an additional patch might be stored alongside the main archive.

Record the complete directory path, not just the filename. For example:

```
/pub/games/quake/mods/actionq2/actionq2.zip
```

Preserve the full path even when the file is no longer available.

## Identify Alternative Copies and Mirrors

Historical FTP archives were frequently mirrored across multiple servers. The same file may survive in several locations, sometimes with different directory paths or filenames.

Use the following approach:

1. Search for the exact filename in FTP search engines.
2. Inspect the known modern mirrors.
3. Search for the filename together with the name of a known archive.
4. Check project websites and news articles for alternative download locations.
5. Compare any recovered copies using file sizes and cryptographic hashes.

Compare file sizes and SHA-256 hashes to identify identical copies. Investigate differences before deciding whether files represent separate releases or repackaged distributions.

Identical files recovered from different mirrors provide separate evidence of distribution. Record each significant location, including the FTP path, mirror name and available dates, under the relevant release in `research/history.md`.

## Use the Wayback Machine to Inspect Historical FTP Interfaces

Many historical FTP servers also offered HTTP interfaces for browsing directories and downloading files. The Wayback Machine may have preserved these HTML directory listings even when the original FTP servers have disappeared.

Search the Wayback Machine for known FTP hostnames and directory paths. You can also try the HTTP version of a known FTP location. For example, if you know an archive was hosted at:

```
ftp://example.com/pub/quake/
```

try inspecting:

```
http://example.com/pub/quake/
```

The actual web interface may use a different hostname or URL structure, so treat this as a lead rather than an assumption.

For example, historical files on `ftp://ftp.cdrom.com/pub/...` may be available via an archived web interface like `http://www.cdrom.com/pub/...`. Searching the Wayback Machine with URLs starting with `cdrom.com/` (without the ftp or http elements) is a handy trick.

Archived directory listings may preserve filenames, file sizes, server timestamps and evidence of changes between captures.

Sometimes the Wayback Machine has captured the files themselves. More often, it has captured only the HTML index pages. Those pages are still valuable because they document which files were available, even when the downloads cannot be recovered.

Compare directory listings from different capture dates. This can help establish when a file first appeared in the archive, when it was removed, or whether a new version replaced an older one.

## Record FTP Findings in the Archival Record

As with the other research sources, findings should be recorded as they are discovered.

For each relevant file, record its filename, release version, FTP hostname, complete directory path, archive or mirror name, and available source dates. Include file sizes, hashes and recovery status when available.

Record whether you recovered the actual file or only found evidence of its existence in a directory listing.

Add the distribution information and supporting references to the relevant release entry in `research/history.md`.

If a file is known to have existed but cannot be recovered, add its filename and historical location to `research/wishlist.txt` and `research/wishlist_urls.txt`.

Preserve the distinction between an original FTP location and a modern mirror. The modern mirror is where you recovered the file. The original FTP path is evidence of where it was historically distributed.

## Summary

Historical FTP archives and their modern mirrors preserve Quake modifications, original directory structures and evidence of distribution. Resources such as Gamers.org, Dukeworld and Quaddicted provide access to surviving collections, while FTP file indexes help locate additional copies.

Investigate archive directory structures, historical HTTP interfaces and alternative mirrors. These sources can reveal missing releases and distribution locations even when the original downloads no longer survive. More advanced techniques, including searching FTP archive indexes, upload summaries and maintenance files, are covered later in this guide.

**Outcome**: You can locate and search historical FTP archives, investigate surviving mirrors and directory listings, and recover missing Quake files. You can also identify historical distribution locations and document the provenance of recovered files.

The next chapter will explore another source of historical information and files: developer websites, personal archives and other surviving online collections.
