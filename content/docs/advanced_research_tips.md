---
title: 21. Advanced Research Tips
weight: 50
---


# 21. Advanced Research Tips

By this point, you should have some experience researching Quake modifications, recovering historical files and building an archive.

You may also have developed a collection of scripts and tools to automate parts of your research.

This chapter shares some of the more advanced techniques I regularly use when investigating difficult archival projects. These are approaches I have developed through experience, particularly when searching for obscure files that have disappeared from their original download locations.

The techniques build on the research methods covered earlier in this guide. Rather than repeat those methods, I want to highlight a few areas that are especially valuable and easy to overlook.

The common theme is that historical file locations contain far more information than they first appear to.

A single download URL might lead to an old directory listing, which reveals additional files, alternative mirrors, earlier releases or an entirely different collection worth investigating.

Learning to recognise and exploit these connections is one of the most useful skills you can develop as a Quake archivist.

## **17.1. Google Does Not Index Everything**

One of the most important lessons I have learned is how limited Google and other general-purpose search engines are when it comes to finding historical files.

You might assume that searching for an exact filename would reveal most publicly available copies of that file.

In practice, this is often not the case.

The more time you spend examining public file archives, FTP mirrors and historical directory listings, the more you realise how much material is missing from Google's index.

Large collections may contain thousands of files that do not appear in search results, even when their directories are publicly accessible.

Other collections may be partially indexed, with some filenames appearing in search results and others completely absent.

This is particularly common with historical FTP archives, directory listings, nested collections and files stored inside compressed archives.

**Do not assume a file does not exist simply because Google cannot find it.**

Use Google to discover websites and possible download locations, but be prepared to investigate those locations manually.

Browse directory structures, inspect file listings and search for filenames within the archives themselves.

If you have programming experience, consider writing tools to download and index directory listings from promising websites.

A simple script can collect filenames and URLs from a public file archive, allowing you to search the collection locally.

For larger collections, this can reveal files that would otherwise remain invisible to general-purpose search engines.

Be respectful when using automated tools. Cache downloaded pages, limit requests, avoid unnecessary downloads and do not overload the servers hosting these collections.

We have already covered manual searching and automation in earlier chapters, but I cannot stress this point enough: **search engines are only one way of discovering files, and they miss an enormous amount of historical material.**

## **17.2. Investigate the Walnut Creek CDROM Archive**

Walnut Creek CDROM operated `ftp.cdrom.com`, one of the most important historical FTP servers for game modifications and other downloadable software.

Its archives included the original idgames collection for Doom and the idgames2 collection for Quake-engine games.

The idgames2 archive is particularly important for Quake research because it was a major distribution location for modifications, maps, tools and other community-created files.

Historical references often point directly to files hosted at `cdrom.com`.

The archive also had an HTTP interface (for a time), which allowed people to browse FTP directories through web pages.

This is valuable because the Wayback Machine preserved many of these historical directory listings.

A file may no longer be available, but an archived directory page can still confirm that it existed, reveal its original filename and provide information about its size or distribution location.

You can also explore historical copies of the archive through its surviving mirrors. Gamers.org continues to host the idgames2 archive and documentation associated with the original collections.




### **Search alternative directory structures**

One complication is that `ftp.cdrom.com` used different directory structures over time.

Some paths were aliases or symbolic links to other directories. Others reflected changes in how material was organised or mirrored.

Historical references to Quake files might therefore contain very different URLs.

For example:

```
ftp://ftp.cdrom.com/pub/quake/quakec/...

ftp://ftp.cdrom.com/.1/idgames2/...

ftp://ftp.cdrom.com/.3/planetquake/...
```

These differences matter when searching historical web archives.

A Wayback Machine capture of one directory path does not guarantee that another path was also captured.

When researching a particular file, record every historical URL you discover, even when the paths appear to refer to the same underlying collection.

Investigate the different paths individually.

One variation may have been archived at a useful date when another was not.

You may also discover directory listings that reveal files that have not appeared in your research elsewhere.

### **Search archive index and maintenance files**

Historical FTP archives often maintained special files that described their contents and recent changes.

These can be extremely useful for reconstructing the existence and distribution of old releases.

Some important filenames and locations to investigate include:

| File or directory              | Research value                                                 |
| ------------------------------ | -------------------------------------------------------------- |
| `pub/idgames2/incoming/`       | Newly uploaded files awaiting moderation or placement          |
| `pub/idgames2/newstuff/`       | Recently added or moderated material                           |
| `pub/idgames2/00alltxt.tar.gz` | Collection of text descriptions associated with archived files |
| `pub/idgames2/00find.gz`       | Historical index of text filenames                             |
| `pub/idgames2/CHANGES`         | Changes to the archive's organisation and structure            |
| `pub/idgames2/LAST.24hours`    | Files recently added or changed within a 24-hour period        |
| `pub/idgames2/LAST.7days`      | Files recently added or changed within a seven-day period      |
| `pub/idgames2/ls-laR.gz`       | Recursive listing of files and directories in the archive      |

Not every file or directory will exist in every historical snapshot or surviving mirror.

Search for archived copies of these resources as well as the current copies available through surviving archives.

The `ls-laR.gz` file is especially useful because it can provide a searchable snapshot of an entire directory tree.

Likewise, a historical `LAST.7days` listing might reveal that a file appeared on the server during a particular week.

These listings do not necessarily establish an original release date, but they provide valuable evidence about when and where files were distributed.

The `CHANGES` file can also help explain why a directory disappeared or why the same material appears under a different path.

Do not restrict your investigation to the individual ZIP file you are looking for. The surrounding directory and its maintenance files can be just as valuable.

## **17.3. Search Historical Mirrors of idgames and idgames2**

The idgames and idgames2 archives were mirrored across many FTP servers around the world.

This provides an important research opportunity.

If you know that a particular file existed in a specific directory on `ftp.cdrom.com`, you can investigate the corresponding directory on other mirrors.

A mirror might no longer host the file, but the Wayback Machine may contain a historical directory listing showing that it was available.

Another mirror might preserve a different version of the file, an earlier directory listing or additional metadata.

Search for mirrors using historical FTP documentation, archived websites and mirror lists maintained by the archives themselves.

Try the historical directory URLs in the Wayback Machine, including HTTP interfaces where they existed.

Browse archived directory listings and look for the files you need.

Compare filenames, sizes, dates and neighbouring files.

An archived listing from one mirror may provide information that is absent from the original server's surviving records.

This is particularly valuable when trying to determine whether a release was replaced, renamed or distributed in more than one form.

### **Mirrors of mirrors**

An additional complication is that `ftp.cdrom.com` mirrored other major file collections, including PlanetQuake material.

Some other FTP servers then mirrored directories from `ftp.cdrom.com`.

This created multiple layers of distribution.

For example, historical paths associated with the idgames2 and PlanetQuake collections included:

```
src.doc.ic.ac.uk/public/Mirrors/ftp.cdrom.com/pub/idgames2/planetquake

sunsite.doc.ic.ac.uk/pub/0-Most-Packages/idgames2/planetquake

task.gda.pl/pub/games/idgames2/planetquake
```

Each represents another location to investigate.


A file originally hosted by PlanetQuake might have been available directly from PlanetQuake, through the Walnut Creek archive and through several mirrors of Walnut Creek.

Each location may have had its own directory structure and historical snapshots.

A file removed from the original PlanetQuake server might still have survived on a secondary mirror.

Likewise, the Wayback Machine might have captured the directory listing of a mirror even if it never captured the original download page.

When you discover that an archive mirrored another archive, treat that relationship as a new research opportunity.

Investigate both the original source and the downstream mirrors.

This is one of the most productive ways to expand a search beyond the obvious download locations.

## **17.4. Search Every Historical PlanetQuake Website Address**

PlanetQuake was a major hosting service for Quake modifications and community projects.

Projects were often assigned their own hosted directories or subdomains.

For example, a modification called QMatrix might have used:

```
planetquake.com/qmatrix
```

However, PlanetQuake's hosting arrangements changed over time, particularly during the GameSpy era.

The same project might have been accessible through several different hostnames or directory structures.

Some historical variations worth checking include:

```
planetquake.com/qmatrix
planetquake.gamespy.com/qmatrix
hosted.planetquake.gamespy.com/qmatrix
qmatrix.planetquake.gamespy.com
dynamic.gamespy.com/qmatrix
dynamic0.gamespy.com/~qmatrix
dynamic1.gamespy.com/~qmatrix
dynamic2.gamespy.com/~qmatrix
dynamic3.gamespy.com/~qmatrix
dynamic4.gamespy.com/~qmatrix
dynamic5.gamespy.com/~qmatrix
dynamic6.gamespy.com/~qmatrix
dynamic7.gamespy.com/~qmatrix
dynamic8.gamespy.com/~qmatrix
```

These are historical URL patterns to investigate, not a guarantee that every project used every address.

When you identify the original PlanetQuake directory for a modification, substitute its project name into these patterns and search the Wayback Machine.

It is worth checking each variation individually.

Often, you will find that several addresses resolve to the same website and were archived around the same dates.

However, this is not always the case.

One address might have captures from an earlier period. Another might contain additional pages, different downloads or snapshots taken after the original hostname stopped working.

You may also discover that an archived website is broken under one hostname but navigable under another.

### **Automate the search**

This is an excellent task to automate.

Write a script that accepts a PlanetQuake project name and generates the known historical URL variations.

Use the Wayback Machine's capture index to identify archived versions of each possible homepage.

Download the relevant HTML pages and compare them.

You can then search those pages for release announcements, download links, filenames and other useful information.

Many captures will be duplicates, so use hashes or content comparison to avoid reviewing identical pages repeatedly.

The goal is to identify unique historical snapshots that contain information missing from the others.

A small reusable tool can make this process much faster, particularly when researching several PlanetQuake projects.

## **17.5. Investigate Every Known Download Directory**

This is one of the techniques that has helped me most over the years.

As you research a modification, you will collect historical URLs where its releases were distributed.

Some may come from original project websites, others from news announcements, FTP archives, mirrors or readmes.

Record all of them.

Importantly, record download locations for both recovered files and releases you have not yet found.

Then examine the directory paths rather than looking only at the individual files.

For example, suppose your research has identified several historical download URLs:

```
http://example.com/quake/mods/qmatrix10.zip
http://example.com/quake/mods/qmatrix11.zip
http://mirror.example.net/planetquake/qmatrix/qmatrix12.zip
```

Remove the filenames to obtain the parent directories:

```
http://example.com/quake/mods/
http://mirror.example.net/planetquake/qmatrix/
```

These directories are now research targets in their own right.

Search for historical captures of each directory in the Wayback Machine.

If a directory listing was archived, inspect it for additional files.

You might discover an earlier version, an incremental patch, a supplementary download or a release that was never mentioned on the project homepage.

You may also discover unexpected files that suggest a different naming convention.

### **Look for patterns across download locations**

Once you have collected several download directories, look for patterns.

Do multiple URLs share the same directory structure?

Does one server appear to be mirroring another?

Are there alternative hostnames that might use the same path?

Could a known PlanetQuake directory have been mirrored through `ftp.cdrom.com` or another historical FTP service?

These relationships can suggest new locations to investigate.

For example, if you know that one PlanetQuake release was copied into a particular FTP mirror directory, investigate whether that directory also contained earlier or later releases.

Search for the same directory on other mirrors.

This approach can turn a handful of historical download URLs into dozens of useful research targets.

### **Automate directory investigation**

This is another excellent opportunity for automation.

A script could accept a list of historical download URLs and:

1. Extract the parent directory from each URL.
2. Remove duplicate directories.
3. Generate known mirror and hostname variations.
4. Search the Wayback Machine for archived directory listings.
5. Download the available HTML listings.
6. Extract filenames and file download URLs.
7. Produce a report of files discovered across the different directories.

You could then compare the report against your known release filenames and wishlists.

This helps identify files that you did not know existed, as well as alternative copies of releases that are still missing.

It also turns your accumulated research into something more powerful than a collection of disconnected links.

**Every historical download URL is a clue to an entire directory, and every directory may contain clues to other releases.**

## **17.6. Get Good at Guessing Historical Filenames**

Searching for missing releases often requires making educated guesses about their original filenames.

This is a skill that improves with experience.

Developers did not always use consistent naming conventions. A modification might use one filename format for its first release and a different format for later versions.

Files were also frequently renamed by the services that distributed them.

BBS operators sometimes shortened filenames to fit older naming conventions. FTP mirrors might rename files to avoid conflicts or make version numbers clearer.

Magazine CDs and shovelware collections sometimes unpacked releases, compressed them again or converted them into other archive formats.

As a result, the filename you are looking for may be different from the one originally published by the developer.

### **Guess version number variations**

Suppose you know that a modification had a release called version 1.2.

Possible filenames might include:

```
qmatrix12.zip
qmatrix120.zip
qmatrix_v12.zip
qmatrix_v1_2.zip
qmatrix1-2.zip
qmatrix_1.2.zip
qmatrix12b.zip
qmatrix.zip
```

The modification might also use an abbreviated name:

```
qm12.zip
qmat12.zip
qmx12.zip
```

These are only possibilities, but searching for them can reveal files that would otherwise remain hidden.

Look at the filenames of known releases and try to infer the developer's naming conventions.

Then generate variations for missing versions.

A script can help produce candidate filenames and search your locally indexed collections.

### **Guess alternative archive formats**

Do not restrict your search to ZIP files.

Historical Quake modifications were distributed in several formats, including:

```
.zip
.rar
.arj
.lzh
.exe
```

A self-extracting executable might contain an otherwise missing release.

A BBS or CD collection might have repackaged a ZIP into a RAR or another archive format.

Search for plausible extension variations when investigating a missing file.

Remember that the presence of a candidate filename does not prove that it contains the release you need.

Download and inspect promising candidates before drawing conclusions.

### **Investigate generic filenames**

Some modifications were distributed using generic filenames such as:

```
qm.zip
qmatrix.zip
quakematrix.zip
```

These are difficult to search because thousands of unrelated files may share the same name.

In these cases, the surrounding directory and distribution source become especially important.

A generic `qm.zip` inside a directory dedicated to a particular modification may be highly relevant.

Inspect the files and their contents rather than dismissing them because their names are uninformative.

You may also find that a collector or CD publisher renamed a release to fit its directory organisation.

### **Search for missing versions**

If you have versions 1.0 and 1.2, consider whether version 1.1 existed.

This is not proof that such a release was published, but it provides a useful research hypothesis.

Search for plausible filenames, historical announcements and references in readmes or changelogs.

Likewise, a changelog might mention fixes introduced in an earlier version whose distribution archive you have not recovered.

Use these clues to generate additional searches.

The key is to become comfortable making informed guesses while keeping guesses separate from established facts.

A candidate filename is a research lead until you find evidence supporting it.

## **17.7. Build a Searchable Collection of Historical File Listings**

As you investigate more archives, you may accumulate hundreds or thousands of historical directory listings.

Rather than search each one manually, consider building a local collection that can be searched repeatedly.

You do not need a complicated database.

A directory containing downloaded HTML files and text listings may be sufficient.

You can use command-line tools or a small script to search for filenames, project names, developer aliases and other distinctive strings.

For more structured searches, extract the filenames and URLs into a CSV file or SQLite database.

Useful fields might include:

- Original filename.
- Full historical URL.
- Parent directory.
- Source archive or mirror.
- File size, when available.
- Listed modification date, when available.
- Archived page URL.
- Wayback Machine capture date.

This allows you to search across many historical archives at once.

For example, you might search for every filename containing a particular abbreviation, identify every mirror that listed a missing ZIP or compare the sizes of files with identical names.

You can also search for directory patterns, which is often more valuable than searching filenames alone.

A local index is particularly useful when you begin another Quake archival project.

The listings you collected while researching one modification may contain valuable information about dozens of others.

Over time, this can become one of your most useful research resources.

## **17.8. Reuse Research Across Archive Projects**

Researching one modification often reveals information about others.

A PlanetQuake directory might contain links to related projects. A developer's personal website might host several modifications. A CD-ROM listing might identify hundreds of Quake files.

Keep these broader discoveries where you can find them again.

For example, you might maintain a personal list of historical FTP mirrors, PlanetQuake hostname variations, unusual file archives and useful Wayback Machine search techniques.

Likewise, keep the scripts you develop for downloading directory listings, generating filenames and comparing archived files.

Try to make these tools reusable by accepting project names, URLs and search terms as arguments rather than hardcoding them for a single archive.

This investment becomes increasingly valuable as you create more archives.

You may revisit an earlier project with a new search tool and immediately discover files that you missed the first time.

You may also notice relationships between projects that were not obvious when researching them independently.

An obscure modification that originally seemed impossible to investigate might become much easier after you have worked on several other projects from the same period.

## **17.9. Follow Unexpected Leads**

The research techniques described in this chapter are systematic, but many worthwhile discoveries begin with something unexpected.

You might find a file in a directory where it does not appear to belong.

A historical mirror might have an unusual naming convention. An old readme might mention a developer alias that leads to another website.

A CD collection might include files from a modification you have never heard of.

Do not ignore these clues simply because they fall outside your immediate search.

Record them in your notes and investigate when they appear promising.

At the same time, avoid following every possible lead indefinitely.

Some connections will produce nothing useful.

A good approach is to capture the information, make a brief assessment and decide whether it is worth pursuing now or saving for later.

As you gain experience, you will become better at recognising which leads are likely to be productive.

The most important skill is not memorising a list of websites or commands. It is learning to recognise relationships between files, directories, mirrors, developers and historical references.

Those relationships are often what lead you to material that conventional searches cannot find.

## **Chapter Summary**

Advanced Quake archival research often involves looking beyond individual files and investigating the historical systems that distributed them.

General-purpose search engines miss large amounts of publicly accessible material, so manual exploration and locally indexed file listings remain important.

The Walnut Creek CDROM archive, its historical directory structures and its network of mirrors provide valuable opportunities for reconstructing old download locations.

PlanetQuake's changing hostnames and directory structures offer similar opportunities, particularly when combined with automated searches of the Wayback Machine.

Recording every known download URL, investigating its parent directory and looking for related mirrors can reveal releases that were not previously known.

Finally, learning to guess historical filenames and recognise repackaged or renamed distributions can help recover files that are otherwise difficult to identify.

These techniques become more effective with experience, and the tools and knowledge developed for one archive can be reused across many others.

**The outcome of this chapter is a collection of advanced research techniques for finding obscure Quake files, reconstructing historical download locations and discovering material that ordinary searches overlook.**