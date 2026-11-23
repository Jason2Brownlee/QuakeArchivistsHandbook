---
title: 6. Design the Archive Structure
weight: 20
---

# 6. Design the Archive Structure

Before you begin substantial research, establish a simple structure for storing what you discover.

During an archival project, you will collect original downloads, historical URLs, release announcements, research notes and clues about missing files. Without an organised structure, these discoveries can quickly become scattered and difficult to manage.

Establishing a simple directory structure before beginning substantial research makes it easier to preserve original files and keep track of what you discover.

The goal of this chapter is to create a working directory that separates the archived files from the research about those files, while remaining simple enough to maintain.

## Keep the structure simple

An archival project does not need a complicated database or elaborate document management system.

For many Quake modification archives, a small collection of directories and text files is sufficient.

I recommend starting with this structure:

```
quake-archive/
    README.md
    bin/
    research/
        history.md
        notes.txt
        wishlist.txt
        wishlist_urls.txt
```

This is deliberately simple. You should be able to understand the structure immediately, even if you return to the project after several months.

You can add more documents and directories as the project grows, but there is no need to anticipate every possible research activity in advance.

I generally recommend markdown (`.md` files) for documentation (e.g. readme and history) as it gives a little more flexibility over plain text. If you are new to markdown, you can get started here:

* [Markdown, Wikipedia](https://en.wikipedia.org/wiki/Markdown)\
    `https://en.wikipedia.org/wiki/Markdown`

## The project `README.md`

The `README.md` file is the main entry point to your archive.

Someone visiting the project should be able to open this file and quickly understand what the archive contains, where to find the files and how the material is organised.

It should provide a concise summary of the project, rather than attempting to document every detail of its history.

A useful README might contain the following sections:

- **Project description:** What modification or collection is being archived?
- **Archive scope:** What material is included and excluded?
- **Available releases:** A list of known releases, their dates and links to recovered files.
- **Archive contents:** A brief description of the files and directories.
- **Research documentation:** Links to the detailed history and supporting research.
- **Credits and references:** Acknowledgements and links to important historical sources.
- **Outstanding gaps:** A brief note about important missing releases or unresolved questions.

For example, a simplified `README.md` for an Action Quake archive might look like this:

```
# Action Quake Archive

A historical archive of the original Action Quake
modification for Quake.

The archive aims to preserve known releases,
supporting files and historical information about
the development and distribution of the project.

## Releases

| Version | Date | File |
|---------|------|------|
| 0.1     | 19970130 | [Download](bin/aq01.zip) |
| 0.5     | 19970228 | [Download](bin/aq05.zip) |
| 1.0     | 19981010 | [Download](bin/aq10.zip) |
| 1.1     | 19981127 | aq11.zip |

## Archive contents

- `bin/`: Recovered original files.
- `research/`: Historical information and research notes.

## Research

- [Release history](research/history.md)
- [Research notes](research/notes.txt)
- [Missing files](research/wishlist.txt)

## Status

Several known releases are still missing.
See the research documentation for details.
```

The example uses fictional release information to demonstrate the layout.

Notice that the README links directly to files in the archive. This makes it easy for someone to browse the project and download a particular release without having to understand the entire research process.

The README should be updated as the archive grows. When you recover a missing release, add it to the release list and link to the corresponding file.

Think of it as the public catalogue for your archive.

## The `bin/` directory

The `bin/` directory contains the actual files you have recovered.

The name is short and convenient, although you could use `files/` or `downloads/` if you prefer.

For a Quake modification archive, this directory might contain file types like `.zip`, `.txt`, `.exe`. and more.

For example:

```
bin/
    aq01.zip
    aq05.zip
    aq10.zip
    aq11_patch.zip
    aq_maps.zip
    aq_server_tools.zip
```

These are examples of possible filenames, not a claim about the actual Action Quake release history.

The important principle is that this directory should contain the files themselves, not descriptions of the files or your research about them.

You might recover a ZIP file from an archived website, find an identical copy on a magazine CD and later discover another copy on an FTP mirror.

Preserve at least one unchanged copy of each distinct file. If multiple recovered files are byte-for-byte identical, you do not need to retain every duplicate in `bin/`. However, record their original filenames and recovery locations in your research documentation.

Files with different contents should be preserved separately, even when they share the same filename.

Avoid casually renaming, modifying or repackaging recovered files. The original filename and contents can be important historical evidence.

If you need to repair a damaged file, extract its contents or create a repackaged version, keep that derived version separate from the original. Document what you changed.

For now, you do not need a complicated directory hierarchy inside `bin/`. A flat directory is often easier to search and maintain when the archive contains dozens or even hundreds of files.

If the collection eventually becomes very large, you can introduce subdirectories for games, releases or file types. Do this when there is a practical reason, not simply because the archive has started to grow.

For example, in the Quake Bot Archive, a separate subdirectory is added to the `bin/` directory for each bot to house quake bot route files that are required but a given bot to navigating popular deathmatch maps:

```
bin/
    reaper/
    frogbot/
    frikbot/
    ...
```


## The `research/` directory

The `research/` directory contains your historical records, research notes, outstanding questions and information about missing files. It is kept separate from the recovered files in `bin/`.

Someone might download the archive simply to play an old modification. They do not necessarily need to read your research notes.

However, someone interested in the history of the modification might want to understand where the files came from, how the release chronology was reconstructed and which versions are still missing.

Keeping the research separate allows both uses.

The initial research directory contains four files:

```
research/
    history.md
    notes.txt
    wishlist.txt
    wishlist_urls.txt
```

Each has a specific purpose.

### `history.md`

The document should provide a chronological account of releases, project websites, historical download locations and supporting references. For now, a simple outline is sufficient; you will fill it out as you establish the archival record.

The aim is to document the project's history with enough supporting evidence that another researcher could independently reconstruct your findings. As the research grows, you may move substantial sections into separate documents.

As the project grows, you may decide to move some of these sections into separate research documents. For now, keeping them together makes the archive easier to manage.

### `notes.txt`

This is your informal working notebook.

Use it to record discoveries, ideas, todos, questions and observations that do not yet belong in the formal historical record.

For example:

```
Action Quake research notes

- Original homepage appears to have been hosted on
  a PlanetQuake subdomain.

- Search Wayback captures around late 1997.

- Possible developer name: John Smith.
  Need to verify identity.

- Found reference to version 0.7 in a news post.
  No download found yet.

- Check Quake magazine CDs from 1998.

- Search Usenet for the filename aq07.zip.
```

These notes do not need to be polished.

You might record something that turns out to be incorrect, make a guess about a filename or write down a search query that you want to try later.

The important thing is to capture ideas and discoveries while they are fresh.

Do not spend time deciding exactly where every observation belongs. Put it in your notes and organise it later when you have enough information.

One useful habit is to include dates when recording important discoveries. This helps you remember when and how a particular research lead emerged.

### `wishlist.txt`

This file records files that you know or suspect exist but have not yet acquired.

It is particularly useful for tracking incomplete releases and missing downloads.

When talking with other quake archivists, you may be asked: "_What files do you need?_" You may immediately share your `wishlist.txt` file in response.

I like to keep my `wishlist.txt` machine readable with comment lines prepended with a `#` and only the filenames exposed. This allows us to later write a script that reads the file and automatically checks resources for reference to wanted files.

For example:

```
# Known missing files

# Referenced in a December 1997 announcement.
aq07.zip

# Mentioned in a contemporary review.
aq10_patch.zip

# Referenced in a server installation guide.
# guessed filename
aq_server_linux.tar.gz
```

You can also record uncertain filenames and possible variations.

For example, an old announcement might mention a file called `aq2_final.zip`, but you have no evidence that this was the exact filename. Record it as a possible filename rather than treating it as confirmed.

As you recover files, update the wishlist and remove or mark the corresponding entries as acquired.

### `wishlist_urls.txt`

This file records historical URLs for files that you have not yet recovered.

These URLs are especially valuable when researching old Quake modifications because the original download locations often disappear.

For example:

```
http://www.example.invalid/files/aq07.zip

http://ftp.example.invalid/pub/quake/aq/aq10.zip

http://planetquake.example.invalid/aq/downloads/aq_patch.zip
```

These are illustrative URLs.

You might discover them in an archived homepage, an old announcement, a readme file or a directory listing.

Preserve historical URLs exactly as found, even when they no longer work. Keep original download locations separate from Wayback Machine captures and alternative mirrors so that the original distribution history remains clear.

Your wishlist URLs may be invaluable when searching archived directories and alternative mirrors, as explained in [Chapter 22: Advanced Website Research](../advanced_website_research.md).

## Keep research evidence and file metadata connected

The initial structure deliberately keeps things simple. However, two important types of information will become increasingly significant as your research progresses.

The first is historical evidence. The second is file metadata.

**Historical evidence** includes archived webpages, release announcements, readmes, directory listings and other sources that support your findings. Record enough information to locate each source again, including relevant URLs and dates.

Initially, you can record references directly in `history.md`. For example, evidence of a release file size and timestamp can be captured from archived HTML pages that show FTP archives. These can be copy-and-pasted into `history.md` under the heading for the given version number:

```
btskn22.txt            04-Nov-96 21:37     7k
btskn22.zip            04-Nov-96 21:39   383k
```

If you begin collecting copious amounts of evidence for a large number of releases, you can add a dedicated directory:

```
research/
    evidence/
        websites/
        announcements/
        readmes/
        screenshots/
        ftp-listings/
```

The second type of information is file metadata, including filenames, file sizes, timestamps, hashes and recovery sources. Initially, this information can be recorded alongside the relevant release in history.md.

You do not need to create a separate metadata catalogue immediately. You can begin by recording this information in the relevant release entry in `history.md`.

As the archive grows, a separate file catalogue may become useful:

```
research/
    files.csv
```

A CSV file can be opened in a spreadsheet or processed with a small script. It also makes it easier to search, sort and compare hundreds of recovered files.

The important point is to keep the actual files in `bin/` and the information describing those files in your research documents.

## Distinguish verified information from research leads

Your research will include both reliable historical evidence and uncertain leads. Distinguish between them so that speculation does not become part of the established historical record.

For example, consider the following statements:

- A surviving ZIP file contains a readme identifying it as version 1.0.
- A contemporary news announcement says version 1.1 was released.
- A forum post mentions a version 1.2, but provides no download or further details.
- You suspect that version 1.3 existed because the filename appears in an old directory listing.

These are four different levels of certainty.

You should avoid turning a plausible research lead into an established historical fact.

A simple approach is to use explicit status labels in your research documents.

| Status      | Meaning                                                             |
| ----------- | ------------------------------------------------------------------- |
| Confirmed   | Directly supported by reliable surviving evidence                   |
| Probable    | Supported by evidence, but some details remain uncertain            |
| Unverified  | A reference or claim has been found but not independently confirmed |
| Speculative | A possibility or research hypothesis                                |
| Unknown     | Insufficient information to make a determination                    |

For example, a release entry might look like this:

```
### Version 1.2

- Date: Approximately March 1998
- Filename: aq12.zip
- File status: Not recovered
- Historical status: Unverified
- Evidence: Mentioned in a forum discussion.
- Notes: The discussion does not include a download link.
```

This tells a future reader that the release is a research lead, not a confirmed recovered file.

You can use the same approach in `notes.txt` and `wishlist.txt`.

As you find stronger evidence, update the status. If a claim turns out to be incorrect, correct it rather than allowing it to remain in the historical record.

## Allow the structure to grow

The directory structure introduced in this chapter is a starting point, not a rigid specification.

As you research a project, you will inevitably discover areas that deserve more detailed investigation.

For example, suppose you are researching a modification and discover that it appeared on several third-party Quake magazine CDs.

You might decide to investigate those CDs systematically. This could involve identifying all known discs, recording their contents, locating disc images and comparing the files they contain.

That research could justify a separate document:

```
research/
    history.md
    notes.txt
    wishlist.txt
    wishlist_urls.txt
    quake-cds.md
```

The new `quake-cds.md` document might contain:

- A list of known Quake magazine CDs.
- Publication dates and magazine issues.
- Links to available disc images.
- Directory paths containing relevant files.
- Files recovered from each disc.
- Duplicate files and differences between versions.
- Outstanding questions about missing discs.

The main history document can then refer to this specialised research rather than containing every detail itself.

Other research activities might justify their own documents:

```
research/
    history.md
    notes.txt
    wishlist.txt
    wishlist_urls.txt
    quake-cds.md
    websites.md
    usenet.md
    ftp-archives.md
    developers.md
```

Add specialised documents only when a research topic becomes substantial enough to justify them.

## Keep working material separate from the published archive

There is an important distinction between the information you collect while researching and the information you eventually publish.

Your working notes might contain:

- Unverified claims.
- Possible filenames.
- Incomplete URLs.
- Speculation about release dates.
- Search queries.
- Personal observations.
- Questions that need further investigation.

These are useful to you, but they are not necessarily appropriate for a public-facing historical record.

The published archive should present information clearly and distinguish confirmed facts from unresolved questions.

For example, you might keep a detailed discussion of conflicting release dates in `notes.txt`, then write a concise explanation in `history.md` once you understand the available evidence.

Similarly, you might maintain a large collection of possible download URLs in `wishlist_urls.txt`, but only include recovered and verified downloads in the public release catalogue.

You do not need to publish every working document. Some archives may benefit from making their research notes public, while others may prefer to publish only the cleaned-up historical record and file catalogue.

The choice is yours.

The important thing is to avoid confusing temporary research material with the finished archive.

## Your first working directory

You are now ready to create the initial directory structure.

For example, you can create the initial Action Quake archive structure using the following commands on macOS or Linux:

```
mkdir -p action-quake-archive/bin
mkdir -p action-quake-archive/research

touch action-quake-archive/README.md
touch action-quake-archive/research/history.md
touch action-quake-archive/research/notes.txt
touch action-quake-archive/research/wishlist.txt
touch action-quake-archive/research/wishlist_urls.txt
```

Add a short project description to `README.md` and record any initial research questions in `notes.txt`. You now have the foundation for developing `history.md` into a detailed historical record.

## Chapter summary

A simple and consistent directory structure makes an archival project easier to research, maintain and publish.

The main ideas from this chapter are:

- Keep the root of the project clean, with only a small number of important files and directories.
- Use `README.md` as the public entry point and catalogue for the archive.
- Store recovered original files in `bin/`.
- Store historical information, references and research notes in `research/`.
- Use `history.md` to document releases, project websites and historical references.
- Use `notes.txt` for informal observations, questions and research leads.
- Use `wishlist.txt` to track missing files and `wishlist_urls.txt` to track their historical download locations.
- Keep verified information distinguishable from unverified claims and speculation.
- Add specialised research documents when a particular topic becomes substantial.
- Keep temporary working material separate from the polished public documentation.

**Outcome:** You have created a working directory and a basic structure for recording discoveries, preserving files and documenting the history of your chosen modification.

In [Chapter 7: Establish the Archival Record](establish_the_archival_record.md), you will begin recording known releases, files, websites, historical locations and references systematically.
