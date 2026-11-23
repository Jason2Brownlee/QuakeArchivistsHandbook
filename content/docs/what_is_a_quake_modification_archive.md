---
title: 3. What is a Quake Modification Archive
weight: 20
---

# 3. What is a Quake Modification Archive

Before creating an archive, it helps to understand exactly what you are trying to preserve.

A Quake modification archive is more than a collection of old downloads. It is a structured record of historical software, its files, releases, developers and history.

For simplicity, this chapter focuses on archiving an individual modification. The same principles apply to the other kinds of projects described in [Chapter 5: Choose an Archive Topic](establish/choose_an_archive_topic.md).

In this section, we'll introduce the key concepts that make up an archive and establish what a successful archive should contain.

## The subject of the archive: A modification

The first thing to understand is that a modification is not necessarily a single downloadable file.

A Quake modification is a project that might consist of many different components:

- **Code and game logic:** Changes to the behaviour and mechanics of the game.
- **Maps and levels:** Custom environments and gameplay areas.
- **Models:** New characters, weapons, objects and other 3D assets.
- **Textures:** Images used to change the appearance of the game.
- **Sound and music:** Audio assets added or modified by the project.
- **Configuration files:** Settings and other files required by the modification.
- **Documentation:** Readme files, installation instructions and development notes.
- **Tools and utilities:** Programs created to support development or use of the modification.
- **Source code:** The original source files, where available.
- **Promotional material:** Screenshots, demonstrations, announcements and other material associated with the project.

A modification might also have multiple versions, development branches, expansions, add-ons and related projects.

For example, a popular modification might have an original release, several patches, a collection of additional maps, a dedicated server version and a later expansion.

All of these might be relevant to its history.

**The important concept is that we are archiving a project and its history, not simply collecting ZIP files.**

## Releases and versions: What was distributed?

A release is a particular distribution of a modification at a particular point in its development.

Modifications were frequently updated, sometimes quite rapidly. Developers released bug fixes, added new features, changed maps and addressed problems reported by players.

A hypothetical modification might have the following release history:

| Version | Description            |
| ------- | ---------------------- |
| 0.1     | Early public beta      |
| 0.5     | Feature-complete beta  |
| 1.0     | Initial stable release |
| 1.1     | Bug-fix update         |
| 1.5     | New maps and features  |
| 2.0     | Major new version      |

These are illustrative versions rather than the actual history of a particular project.

It is important to understand that releases were not always distributed as complete packages.

A developer might distribute:

- A complete installation package.
- An incremental patch that updates an earlier version.
- A collection of additional maps.
- A new model or asset pack.
- A server-side update.
- A supplementary tool or utility.

Consequently, finding a file associated with a modification does not necessarily mean you have found a complete release.

There is also an important distinction between several different dates:

- **Version date:** The date associated with a particular version.
- **Release date:** When the developer made the release available.
- **Distribution date:** When a particular copy was distributed, perhaps on a magazine CD.
- **File date:** A timestamp associated with the file itself.

These dates can differ considerably. For example, a magazine CD distributed in October might contain a modification originally released in July.

An archive should preserve these distinctions wherever possible.

## The historical record: What happened and when?

An archive should preserve more than the files themselves. It should also attempt to reconstruct the history of the modification.

This means documenting the sequence of releases, announcements, updates and other significant events.

For example, a hypothetical modification might have the following chronology:

**Example modification chronology**

1. **March 1998**

   First public beta announced on a Quake community website.
2. **June 1998**

   Version 1.0 released with five custom maps.
3. **October 1998**

   Version 1.1 released with several bug fixes.
4. **February 1999**

   Version 2.0 released with a new game mode.
5. **August 1999**

   Final known release distributed through an FTP mirror.

This chronology provides a useful overview of the project's development.

Ideally, it should answer questions such as:

- When was the modification first announced?
- When was the first public release?
- What versions were released?
- What changed between releases?
- Where were the releases distributed?
- Who contributed to the project?
- When did development appear to stop?

Of course, historical records are rarely complete.

Some releases might be missing entirely. Others might have uncertain dates or incomplete descriptions. There might even be references to versions that have never been recovered.

The objective is to reconstruct the most complete history possible from the surviving information, while clearly identifying gaps and uncertainties.

## Historical evidence: How do we know?

Historical archiving involves making claims about events that happened decades ago.

For example, you might want to establish that a particular version of a modification was released in June 1998.

How do you know?

Perhaps you found an announcement on an old website. Perhaps a magazine reviewed the release in July. Perhaps the original readme file contains a date.

These are examples of historical evidence.

Potential sources of evidence include:

- Original release announcements.
- Archived websites.
- FTP directory listings.
- Magazine CD contents.
- Readme files.
- File timestamps.
- Developer statements.
- Contemporary reviews and news articles.
- Forum discussions and mailing lists.
- Screenshots and other contemporary material.

Not all evidence is equally reliable.

For example, an original release announcement is generally stronger evidence of a release date than a timestamp inside a ZIP archive. File timestamps can be changed, preserved incorrectly or affected by the process used to distribute a file.

Similarly, a forum post might mention a forthcoming release without confirming that it was actually published.

An archive should distinguish between what is known, what is reasonably inferred and what is uncertain.

It should also preserve references to the evidence supporting its historical claims.

**The goal is not to create a plausible history. It is to reconstruct the most accurate history supported by surviving evidence.**

## Files and artefacts: What exactly are we preserving?

The actual files are the heart of a software modification archive.

The objective is to preserve original downloadable files so that people can retrieve and use the modification, ideally in the same form in which it was originally distributed.

However, simply collecting files is not enough. Each file needs to be identifiable.

Consider some of the information that might be associated with a file:

| Attribute   | Example                |
| ----------- | ---------------------- |
| Filename    | `mod_v1.0.zip`         |
| File size   | 4.2 MB                 |
| Format      | ZIP archive            |
| Release     | Version 1.0            |
| Date        | June 1998              |
| Source      | Original FTP server    |
| Checksum    | SHA-256 hash           |
| Description | Initial public release |

This information is called file metadata. It helps describe, identify and distinguish individual files.

A particularly important concept is the checksum, or file hash. This is a value calculated from the contents of a file. It can be used to identify identical files and detect whether two files have different contents.

For example, two files might have different filenames but identical contents. Conversely, two files might have the same filename but contain different releases.

These distinctions matter when dealing with old software that has been copied, renamed and redistributed across many websites.

Another important concept is provenance: the history of where a file came from.

A file recovered from an original developer's website has a different provenance from one recovered from an unknown FTP mirror. Both might be valuable, but knowing their origins helps establish confidence in their authenticity.

Finally, it is useful to distinguish between:

- **Original artefacts:** The files as they were originally distributed.
- **Derived artefacts:** Files that have been modified, repaired or repackaged.
- **Metadata:** Information describing the files.
- **Evidence:** Historical material supporting claims about the files and their origins.

Where possible, original files should be preserved independently of any modifications made during archival work.

## The finished archive: What does it contain?

We can now bring these concepts together.

A useful modification archive should contain several complementary components.

| Component           | Purpose                                              |
| ------------------- | ---------------------------------------------------- |
| Project information | Explains what the modification is                    |
| Release chronology  | Documents its development and releases               |
| Release records     | Describes individual versions                        |
| Original files      | Makes the software available                         |
| File metadata       | Identifies and describes individual files            |
| Historical evidence | Supports claims about the project                    |
| Credits             | Recognises developers and contributors               |
| References          | Connects the project to surviving historical sources |

The archive should also be publicly accessible, easy to navigate and searchable.

Ideally, someone should be able to visit the archive, find a particular modification, understand its history, identify a particular release and download the corresponding files.

The archive should be inexpensive or free to host and straightforward to maintain over time.

It should also be possible for other people to contribute missing files, historical information and corrections.

The result is something more useful than a folder of old downloads. It is a structured, publicly accessible historical record of a creative project.

## Levels of archival completeness

One final concept is worth understanding: not every archive will be equally complete.

Some modifications have been extensively documented and have many surviving releases. Others might have only one known download and a handful of references in old forum discussions.

This doesn't mean the second project isn't worth archiving.

It is useful to think about archival completeness in three broad levels.

Level 1

**Basic preservation**

The project has been identified, perhaps one original file has been preserved, and basic information about the modification has been documented.

Level 2

**Documented archive**

Multiple releases have been preserved, file metadata has been recorded, and a chronology has been reconstructed using available historical evidence.

Level 3

**Comprehensive historical archive**

Known releases have been systematically documented, files have been verified, provenance has been recorded, historical evidence has been retained, and gaps in the historical record have been identified.

These are not formal archival standards. They are simply a useful way to think about the completeness of an archive.

An archive does not need to be comprehensive to be valuable. Even preserving one otherwise-lost release can make a meaningful contribution.

## Summary

A Quake modification archive is a structured collection of files and historical information about a modification and its development.

To understand what we are building, remember these six concepts:

1. **The modification:** The project and everything associated with it.
2. **The releases:** The different versions and distributions of the project.
3. **The chronology:** The sequence of events in the project's history.
4. **The evidence:** The surviving information that supports historical claims.
5. **The artefacts:** The actual files, their metadata and their provenance.
6. **The archive:** The organised, publicly accessible record that brings everything together.

With these concepts established, we now have a clear picture of what we want to create.

[Chapter 4: How to Create a Quake Modification Archive](how_to_create_a_quake_modification_archive.md) outlines the practical process, from researching a modification and recovering files to organising and publishing the finished archive.

