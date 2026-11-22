---
title: 13. Search FTP Archives and File Indexes
weight: 60
---

# 13. Search FTP Archives and File Indexes

Previous chapters explored project websites, gaming news archives, Usenet, CD-ROM collections and modern search engines. Another important source of historical Quake files is the FTP archive.

During the 1990s, FTP servers were a major way to distribute game modifications, maps, utilities, patches and other community-created content. Many of these servers are no longer online, but copies of their contents survive in modern mirrors and historical collections.

This chapter explains how to find those surviving archives, search their directory structures, use FTP file indexes, and recover evidence about where and when files were distributed.


## Understand Historical FTP Archives

FTP (File Transfer Protocol) was widely used to distribute files before modern web hosting and download platforms became common.

Quake communities relied on a network of FTP servers and mirrors. Developers uploaded releases to project websites or community archives, and those files were often copied to several mirrors around the world. News sites and project homepages frequently linked directly to these downloads.

Several important historical archives became well-known distribution locations:

- **idgames2** was a major archive of files for Quake-engine games. It included Quake maps, modifications, utilities and other content. Initially hosted on `cdrom.com` and later `gamers.org`.
- **PlanetQuake** was a major Quake community website and hosting service. It hosted individual modification websites and maintained an FTP archive of their files.
- **Telefragged** was another Quake community website and hosting service, with downloadable modifications and related material.
- **Games Domain** was a general PC gaming website that also maintained downloadable game files.

The distinction between these archives is important. PlanetQuake and Telefragged hosted individual community projects, while idgames2 was organised primarily as a central file archive. These different arrangements are reflected in their directory structures, which can help guide your research.

These names refer to archives and distribution services, not individual modifications. A modification might have been hosted on its developer's website, submitted to a central archive, and copied to several mirrors.

This distinction matters when reconstructing a project's history. Finding a file in an archive tells you where a copy was distributed. It does not necessarily identify the original developer or the first place the file was published.

## Start with Modern Mirrors of Historical Archives

A useful starting point is to look for modern mirrors of historical FTP archives. These are surviving copies of older directory trees, sometimes preserving much of the original organisation.

Several useful collections include:

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

You can download a compressed archive file that contains a full and up-to-date list of all files and directories in the archive here:

- https://www.quaddicted.com/files/ls-goalR_cut.xz

### Understand how the archives organise their files

Different archives used different approaches to organising their contents. Understanding these arrangements makes it easier to find files and reconstruct the distribution history of a modification.

**PlanetQuake and Telefragged organised files around hosted projects.**

Both services hosted individual Quake community websites on their networks. Their FTP directory structures often reflect this arrangement, with directories corresponding to particular hosted projects or websites.

A project directory may contain more than just downloadable release files. It might also include readmes, screenshots, website resources, patches, maps and other files associated with that project.

When you find a directory belonging to a particular modification, inspect the entire directory rather than looking only for a known release filename. It may contain additional versions or files that were never mentioned in the project's news announcements.

**idgames2 organised files by game and content category.**

Rather than organising everything around hosted project websites, idgames2 generally categorised files by content type, game or modification category. You will encounter directories for maps, QuakeC modifications, utilities and other types of content.

Some useful locations in the modern Gamers.org archive include:

- [Quake 1 QuakeC modifications](https://www.gamers.org/pub/idgames2/quakec/)\
	`https://www.gamers.org/pub/idgames2/quakec/`
- [Quake 2 files](https://www.gamers.org/pub/idgames2/quake2/)\
	`https://www.gamers.org/pub/idgames2/quake2/`

This means that searching idgames2 often requires looking in the appropriate category rather than searching for a project-specific directory.

**Use the archive structure to guide your search.**

On PlanetQuake and Telefragged, look for the modification's project directory. In idgames2, look for the relevant game and content category, then search within it.

In all cases, inspect neighbouring directories and subdirectories. The archive's organisation may reveal additional releases, patches, documentation and related files that a filename search alone would miss.

Do not assume that every mirror is complete or that its contents are identical to the original server. Different mirrors may have been created at different times, may contain different subsets of files, or may have been updated independently.

These collections are useful because they preserve more than individual downloads. They often retain directory names, subdirectories and original filenames that help establish how files were distributed.

## Search FTP File Indexes

Some websites index files available on public FTP servers. These search engines are particularly useful for two purposes:

1. Finding alternative locations for files you already know about.
2. Discovering additional releases that you may not have encountered during earlier research.

Two useful examples are:

- [FileMood](https://filemood.com/)\
	`https://filemood.com/`
- [Mamont's Open FTP Index](https://www.mmnt.net/)\
	`https://www.mmnt.net/`

Search engines of this kind can help discover files across multiple FTP servers and indexed directories. Their coverage varies, and they may not include every historical archive.

Start with filenames discovered during earlier research. Search for:

- Original release filenames.
- Alternative filename spellings.
- Versioned filenames.
- Patch and update filenames.
- Filenames of distinctive files found inside recovered archives.
- Team names and project names.

For example, if earlier research identified `actionq2.zip`, search for that exact filename. Then try related forms such as `actionq2`, `actionq2_1.5.zip`, or distinctive filenames found inside the archive.

Searching for known filenames can reveal copies that a project-name search would miss. A mirror might contain the original archive under its original filename without mentioning the modification anywhere else.

It can also reveal releases you were not previously aware of. For example, a search might find `actionq2_1.6.zip` when your research has only identified versions 1.4 and 1.5. Treat this as a lead to investigate. Check the file contents and supporting evidence before adding it to the project's release history.

### Accessing FTP Servers

Some FTP search engines provide links directly to the FTP server and directory containing a matching file. You may need an FTP client to browse these locations or download the files.

Modern web browsers generally no longer support direct FTP access, so a dedicated FTP client is often required. One popular open-source option is [FileZilla](https://filezilla-project.org/) (`https://filezilla-project.org/`).

When connecting to a public FTP server, try anonymous access. Typical connection details are:

- **Host:** The FTP server hostname from the search result.
- **Username:** `anonymous`
- **Password:** Your email address.

Some servers accept any password for anonymous access, while others may require an email address or another value. Follow any instructions provided by the server.

Once connected, browse the directory structure and inspect the files. You can download individual files or directory listings for further investigation.

Treat search results as leads rather than definitive evidence. Follow them to the actual directory or file where possible, inspect the contents, and record the full FTP hostname and directory path. Do not rely only on the search engine's result page, since its index may be incomplete or outdated.

Add a practical search workflowExplain what to record from FTP results.

## Inspect FTP Directory Structures

A directory listing is an important historical record. Old FTP archives often contain files in directory structures that reflect their original distribution arrangements.

For example, an archive might organise files by game, content type, project, developer, or release category. A Quake archive could contain directories for maps, utilities, modifications, demos and patches.

A directory listing can provide useful evidence about:

- Which files were available.
- How files were organised.
- Which versions were distributed together.
- Where a particular project was hosted.
- Whether additional releases might be present.

When you locate a relevant directory, inspect its parent directory and neighbouring directories as well. A modification may have been stored in a general `mods/` directory, while related patches or documentation were placed elsewhere.

Look for files with names such as `README`, `INDEX`, `00index.txt`, or other descriptive text files. These may explain the archive's organisation or provide additional information about individual downloads.

Also inspect directory listings for files that you have not yet identified. A release might have a different filename from the one mentioned in a news article, or an additional patch might be stored alongside the main archive.

Record the complete directory path, not just the filename. For example:

```
/pub/games/quake/mods/actionq2/actionq2.zip
```

This path is useful evidence of the file's historical distribution location. Even if the file itself is no longer available, the directory location can help establish where it was hosted.

## Identify Alternative Copies and Mirrors

A file found in one archive may also exist in several other locations.

Historical gaming archives often maintained mirrors to distribute download traffic across multiple servers. A file might appear under the same filename in several countries, or be copied into a different archive with a different directory structure.

Use the following approach:

1. Search for the exact filename in FTP search engines.
2. Inspect the known modern mirrors.
3. Search for the filename together with the name of a known archive.
4. Check project websites and news articles for alternative download locations.
5. Compare any recovered copies using file sizes and cryptographic hashes.

If two copies have the same SHA-256 hash, they are identical at the byte level. If their hashes differ, inspect the files before deciding whether they are different releases, modified copies, or simply repackaged archives.

Do not discard duplicate copies immediately. Their locations may provide useful evidence about distribution history. A file found on a developer's original FTP server and a file found on a community mirror are the same archival object in terms of content, but the two locations tell different parts of its history.

Record each significant location in `research/history.md` under the relevant release. Include the original FTP path, the mirror name, the recovered URL, and any available dates or other evidence.

## Use the Wayback Machine to Inspect Historical FTP Interfaces

An advanced technique is to look for HTTP interfaces to historical FTP archives.

Many FTP servers also provided a web interface that allowed visitors to browse directories and download files through a browser. These interfaces often exposed directory listings as ordinary HTML pages.

Some of these pages were captured by the Wayback Machine:

`https://web.archive.org/`

This creates another opportunity for research. Even when the original FTP server and its files are no longer available, archived HTML directory listings may survive.

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

Archived directory pages can reveal:

- Filenames and directory names.
- File sizes.
- Directory organisation.
- Dates displayed by the FTP server.
- Files that were present at particular points in time.
- Changes between archived directory listings.

Sometimes the Wayback Machine has captured the files themselves. More often, it has captured only the HTML index pages. Those pages are still valuable because they document which files were available, even when the downloads cannot be recovered.

Compare directory listings from different capture dates. This can help establish when a file first appeared in the archive, when it was removed, or whether a new version replaced an older one.

Remember that a Wayback capture date is the date the page was archived, not necessarily the date the file was uploaded or released.

## Investigate the `incoming/` Directory

Some historical FTP archives provided an `incoming/` directory where users could upload files before they were reviewed and moved into the main archive.

These directories are particularly interesting because they may preserve files that were submitted but never incorporated into the organised collection.

Look for archived versions of `incoming/` directories and their listings. They may contain:

- New releases awaiting review.
- Files that were later moved into another directory.
- Alternative versions of existing releases.
- Submissions that never appeared in the main archive.
- Files with timestamps that help narrow down a release period.

An `incoming/` directory can be messy. Filenames may be temporary, incomplete or poorly organised. Do not assume every file was publicly released or officially accepted into the archive.

Nevertheless, these directories can reveal material that is missing from the main collection.

## Look for FTP Archive Index and Upload Summary Files

Some FTP servers maintained special files that summarised their contents or recent uploads. These files can be especially useful when researching historical releases because they provide snapshots of what was available at a particular time.

Examples include:

- `ls-laR.gz`: A compressed recursive directory listing of files on the server. Different copies may represent snapshots taken at different times.
- `LAST.24hours`: A listing of files uploaded during the previous 24 hours.
- `LAST.7days`: A listing of files uploaded during the previous seven days.
- `00alltxt.tar.gz`: An archive containing text files from the server, potentially including readmes, documentation and other useful material.

The exact filenames and formats varied between servers. Look for similar index, listing, upload summary and documentation files when inspecting an archive.

These files can provide evidence about what might have been released and when.

For example, an archived `ls-laR.gz` file may show that `actionq2.zip` existed in a particular directory at the time the listing was generated. A `LAST.7days` file may show that it was recently uploaded.

The `00alltxt.tar.gz` archive can be particularly useful because it may contain readmes and other documentation that are otherwise difficult to locate. These documents can identify project names, version numbers, authors, release dates and original download locations.

When using these files, record their own filenames, source locations and available dates. A directory listing is a snapshot, not a definitive record of the exact upload or release date. Similarly, an upload summary describes activity according to the server's own reporting period.

If you recover a compressed listing or text archive, preserve the original file in your research materials. You can extract a working copy for searching without modifying the original.

## Research the CD-ROM.COM FTP Archive and Its Mirrors

One particularly important historical source for Quake 1 modifications was the Walnut Creek CDROM (`cdrom.com`) FTP archive.

The archive hosted a large collection of Quake-related files, commonly encountered under paths such as:

```
/pub/idgames2/
```

The archive was mirrored by servers around the world. Its welcome message sometimes listed alternative mirrors, including their locations and directory paths.

For example, an archived welcome message from `http://www.cdrom.com/pub/idgames2/`, captured on 10 February 1997, included entries such as:

```
         Welcome to the idgames2 archives at this ftp site
    Games using the Quake engine by id Software are covered here

*** ATTENTION: To reduce the load on this machine and           ***
***            provide faster access for all users,             ***
***            please check the following list for a            ***
***            mirroring site closer to you and use it.         ***
***                                                             ***
*** Ohio         ftp.lame.org/mirrors/quake_stuff/              ***
*** Pennsylvania ftp.epix.net/pub/idgames2/                     ***
*** New York     ftp.gamers.org/pub/games/idgames2/             ***
*** UK           sunsite.doc.ic.ac.uk/packages/idgames2/        ***
***              ftp.compulink.co.uk/pub/games/id/quake/        ***
*** Sweden       ftp.sunet.se/pub/pc/games/idgames2/            ***
***              ftp.edu.sollentuna.se/pub/games/quake-stuff/   ***
*** Finland      ftp.sci.fi/pub/idgames2/                       ***
*** Austria      flinux.tu-graz.ac.at/pub/idsoftware2/          ***
*** Poland       ftp.task.gda.pl/pub/games/idgames2/            ***
*** Portugal     ftp.telepac.pt/pub/idgames2/                   ***
*** S. Africa    ftp.global.co.za/pub/quake/                    ***
***              ftp.is.co.za/games/id2/                        **
*** Australia    ftp.powerup.com.au/pub/games/quake/ Brisbane   ***
***              ftp.livewire.com.au/pub/idgames2/   Brisbane   ***
***              ftp.pnc.com.au/pub/idgames2/        Sydney     ***
***              ftp.questnet.net.au/idgames2/       Brisbane   ***
***              ftp.bf.rmit.edu.au/pub/quake/cdrom/ Melbourne  ***
*** Brazil       ftp.iis.com.br/pub/mirror/Quake/               ***
...
```

This list is valuable for several reasons.

First, it identifies historical mirror servers that may still have surviving copies or references to the original archive. Second, it provides the directory paths used by those mirrors. Third, it helps establish the geographical distribution of the archive and the existence of multiple copies at a particular point in time.

Use these historical mirror lists as a source of further research leads. Search for the hostname and directory path, check whether a modern mirror survives, and inspect archived HTTP interfaces where available.

Some of these mirrors also had web-accessible directory listings. Those pages may have been captured by the Wayback Machine, providing another way to inspect their contents.

This is especially useful for Quake 1 research, where the `idgames2` archive and its mirrors were important distribution locations.

## Record FTP Findings in the Archival Record

As with the other research sources, findings should be recorded as they are discovered.

For each relevant file, record:

- Project and release version, if known.
- Original filename.
- FTP hostname and full directory path.
- Archive or mirror name.
- Recovered download URL, if available.
- File size and SHA-256 hash.
- Any dates shown in the directory listing.
- The date of an archived listing, if using the Wayback Machine.
- Whether the file itself was recovered or only its listing was found.
- Any related files or alternative copies.

Add the relevant distribution information to the release entry in `research/history.md`. Record the FTP archive, mirror or historical listing as a source in `research/lists/references.md`.

If a file is known to have existed but cannot be recovered, add its filename and historical location to `research/wishlist.txt` and `research/wishlist_urls.txt`.

Preserve the distinction between an original FTP location and a modern mirror. The modern mirror is where you recovered the file. The original FTP path is evidence of where it was historically distributed.

As always, be careful with dates. A file's directory timestamp, an archived listing's capture date, and the date of a release announcement are different pieces of evidence. Record each separately rather than treating them as interchangeable.

## Summary

FTP archives preserve an important part of the historical distribution network for Quake modifications. Modern mirrors such as Gamers.org, Dukeworld and Quaddicted provide access to surviving collections, while FTP search engines can help locate files by their original filenames.

Directory listings are valuable archival evidence in their own right. They reveal how files were organised, which releases were available together, and where projects were distributed. Historical HTTP interfaces, `incoming/` directories, upload summaries and recursive directory listings can provide additional evidence, even when the original downloads are no longer accessible.

The next chapter will explore another source of historical information and files: developer websites, personal archives and other surviving online collections.
