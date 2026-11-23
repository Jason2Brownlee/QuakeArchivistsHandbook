---
title: 17. Verify, Classify and Connect Discoveries
weight: 1
---

# 17. Verify, Classify and Connect Discoveries

By this stage, you should have recovered files from a variety of sources, including original project websites, news archives, FTP servers, magazine CDs, community collections and individual contributors. You may also have accumulated historical webpages, readme files, announcements and other evidence.

However, finding a file does not necessarily mean you know what it is.

A file might have an unfamiliar name, belong to an unknown release, be a duplicate of something already recovered or contain only part of a modification. Two files with the same name might contain different releases, while two differently named files might be identical.

This chapter is about examining recovered material closely, determining what it represents and connecting it to the historical record.

This is an iterative process. Every new discovery can change your understanding of the project's history, including the interpretation of files you recovered earlier.

## Maintain the distinction between files and releases

One of the most important distinctions in archival research is the difference between a file and a release.

A release is a particular distribution of a modification by its developers. A file is an artefact that might contain that release, part of that release or something derived from it.

For example:

- The same release might be distributed under several different filenames.
- The same filename might be used for several different releases.
- A release might be distributed as a ZIP archive, an executable installer or a collection of loose files.
- A release might be repackaged by a third party without changing its contents.
- A later release might contain only a patch that needs to be applied to an earlier version.
- A magazine CD might contain an extracted copy of a release rather than the original archive.

This distinction is important when documenting the history of a modification. You should not automatically interpret every recovered file as a separate release.

Instead, identify the underlying release or distribution that each file represents, and document the relationship between the two.

## Identify duplicate files

The first task is to determine which recovered files are identical.

This is particularly important when you have obtained files from multiple sources. The same ZIP archive might appear on an original project website, several FTP mirrors, a magazine CD and a modern community archive.

**Compare file hashes**

Calculate a SHA-256 hash for every recovered file. Files with matching SHA-256 hashes are byte-for-byte identical.

For example, you might find:

```
actionq2.zip
    SHA-256: abc123...

aq2.zip
    SHA-256: abc123...

actionq2_download.zip
    SHA-256: abc123...
```

Despite having different filenames, these are identical files. You only have one unique artefact, recovered from three different locations.

Record the different filenames and recovery sources, but avoid treating them as three separate releases.

**Identify repackaged files**

Not every duplicate will have an identical hash.

Someone might have extracted a ZIP archive and created a new ZIP containing exactly the same files. The resulting archive will have a different hash, even if the contents are identical.

Other differences might include:

- Different directory structures.
- Additional documentation.
- Changed compression settings.
- Different file ordering.
- Modified timestamps.
- An updated readme file.
- An additional installer or launcher.

To investigate these cases, extract the archive contents and compare the individual files.

If every meaningful file is identical, the two archives might represent the same release packaged differently. However, document the differences rather than assuming that the archives are interchangeable.

**Look for nested archives and installers**

Historical software collections sometimes contain an executable that extracts another archive, or an executable installer that places files into a directory.

For example, a magazine CD might contain an executable called `actionq2.exe` that extracts a ZIP archive or installs a modification.

Inspect these files to determine what they contain. If possible, extract the embedded files and compare them with other recovered releases.

Do not assume that an executable is the original developer distribution. It might be a third-party repackaging created for a magazine CD or another software collection.

Record the relationship between the executable and its extracted contents.

## Distinguish different releases

Once you have identified obvious duplicates, examine the files that might represent different releases.

This can be surprisingly difficult because developers frequently reused filenames.

For example, a developer might upload a corrected version of `actionq2.zip` without changing the filename. An FTP mirror might also contain an older copy under the same name.

Consequently, filenames and file sizes alone are not sufficient to establish whether two files represent the same release.

**Compare archive contents**

Start by listing the contents of each archive.

For ZIP files, you can use:

```
unzip -l actionq2.zip
```

For TAR archives, use:

```
tar tvf actionq2.tar
```

These commands display the files contained within an archive, including information such as filenames, sizes and timestamps. Note, commands like `tar tvf filename` work on many archive types, including self-extracting executables.

Compare the resulting listings.

Look for files that have been added, removed or renamed. Pay particular attention to readme files, changelogs, configuration files, maps and other distinctive project assets.

**Compare individual file hashes**

For more reliable comparisons, calculate hashes for the files inside each archive.

For example, two releases might contain the same maps and models but different executable files or readme documents. This could indicate a minor update rather than an entirely separate release.

You can also identify individual files that have been copied unchanged from an earlier release.

**Examine timestamps**

Archive listings often contain internal file timestamps. These can provide useful clues about the sequence of releases.

For example, one archive might contain files dated March 1998, while another contains modified files dated April 1998.

However, timestamps should be treated as supporting evidence rather than definitive dates. They can be affected by copying, repackaging, extraction, incorrect system clocks and archive creation tools.

A collection of timestamps can help establish a likely sequence, but should not be used in isolation to assign a release date.

**Distinguish releases with the same version number**

Sometimes you will discover two different distributions that both claim to be the same version.

This might happen because a developer uploaded a corrected release without changing the version number. It might also happen because a third party modified or repackaged the original distribution.

Do not invent new version numbers to resolve the ambiguity.

Instead, distinguish the recovered artifacts using an archival suffix.

For example:

```
actionq2_15_v1.zip
actionq2_15_v2.zip
```

The suffixes distinguish two different recovered distributions associated with version 1.5. They do not imply that the developer officially released versions 1 and 2.

Document the original filenames, differences and evidence in `history.md`.

## Compare files with different names

Different filenames do not necessarily indicate different content. Files may be renamed by mirror administrators, repackaged for software compilations or distributed under alternative names.

As described earlier, compare SHA-256 hashes first, then inspect archive contents and individual file hashes when necessary.

Preserve the original filenames in your research records. A filename can itself be useful historical evidence, particularly when it appears in contemporary news articles, FTP listings or download announcements.

## Verify archive contents

A successful download does not necessarily mean that you have recovered a complete or valid file.

Files can be truncated, corrupted or incorrectly transferred. Some archives may also be incomplete because the original developer uploaded them incorrectly.

You should verify recovered archives before treating them as valid archival copies.

**Test archive integrity**

For ZIP files, use:

```
unzip -t actionq2.zip
```

This checks whether the archive can be read and whether its contents pass the available integrity checks.

For other archive formats, use the corresponding test or listing commands. For example:

```
tar tvf actionq2.tar
```

A successful listing is a useful indication that the archive can be read, although it does not necessarily verify every file's contents.

**Inspect file sizes**

Compare the recovered file size with historical references where available.

An old FTP listing, download catalogue or news article might record the expected size of a release.

If your recovered file is substantially smaller, investigate whether it is incomplete.

A partial download might still contain some recoverable files, but it should not be presented as a complete release.

**Check for missing files**

Compare the archive contents with historical descriptions, readme files and other recovered copies.

For example, a release announcement might describe several maps, while your recovered archive contains only one. This could indicate an incomplete distribution, a separate map pack or an incremental release.

Do not assume that every discrepancy indicates corruption. It may reflect how the original modification was distributed.

**Record the verification results**

Document whether an archive was successfully tested, whether its contents could be extracted and whether any problems were found.

If an archive is corrupted but contains recoverable files, preserve it in its original form. You can separately extract the recoverable contents and document what was recovered.

Do not silently replace a corrupted original with a repaired version.

## Connect files to known releases

After examining recovered files, determine which known release they belong to.

This is where the research from previous chapters becomes particularly valuable.

You might have a file with no useful filename, but its contents could match a known release. Alternatively, a readme might identify a version number that was not previously known.

Look for evidence in several places:

- Readme files and changelogs.
- Version numbers embedded in files.
- Internal archive timestamps.
- Filenames and directory structures.
- File sizes and hashes.
- Historical download URLs.
- News announcements and release descriptions.
- FTP directory listings.
- Magazine CD catalogues.
- References in other recovered releases.

Try to connect each recovered artifact to an entry in `research/history.md`.

Sometimes the connection will be obvious. A readme might explicitly identify the modification and version number, and the archive contents might match a contemporary release announcement.

Other times, you will need to make an educated guess.

For example, you might recover a file from an FTP mirror with no readme or version number. Its contents might closely match a known release, except for one additional map. It could be a later revision, an unofficial modification or a separate map pack.

Record the evidence and explain your interpretation. Do not force every recovered file into an existing release entry if the relationship is unclear.

**Look for missing releases**

Comparing recovered files can also reveal gaps in the release history.

Suppose you have identified versions 1.0 and 1.2, but discover an archive that appears to contain an intermediate set of files. It might represent version 1.1.

Look for additional evidence before assigning it a version number. Search historical news archives, FTP listings, readme files and other sources for references to the suspected release.

Even when you cannot identify the exact version, document the possibility in `history.md` and add relevant leads to your research notes.

## Identify files with uncertain origins

Not every recovered file will have a clear provenance.

You might find a ZIP archive on a modern file-sharing service, with no accompanying description or historical download information. Its contents might appear to be an old Quake modification, but you may have no evidence of who created it or where it originally came from.

These files can still be valuable.

The important thing is to distinguish what you know from what you suspect.

For each uncertain file, record:

- Where you obtained it.
- The filename and file size.
- Its SHA-256 hash.
- Any identifying information inside the archive.
- The project or release it might belong to.
- Other files with similar contents.
- Your current interpretation.
- Any unresolved questions.

Use the available evidence to make a tentative classification, but leave room for alternative explanations. A file initially identified as an unofficial mirror might later prove to be a beta version or a modified distribution.

Record your current interpretation without presenting it as an established fact.

## Resolve conflicting release dates

Return to the date distinctions established in Chapter 7. An announcement date, a file upload timestamp, a mirror distribution date and a CD publication date may differ because they describe separate events.

Record each date according to what its evidence establishes rather than treating every timestamp as a release date. When different sources appear to provide conflicting dates for the same event, investigate the discrepancy before deciding which interpretation is best supported.

**Investigate discrepancies**

Sometimes conflicting dates reveal something more interesting.

A developer might upload a release, discover a problem and upload a corrected version under the same filename. A mirror might retain the original copy while another mirror receives the replacement.

This can result in two different files with the same name and apparent release date.

Compare their contents, timestamps, hashes and associated documentation. Look for evidence of a corrected release, replacement upload or unofficial repackaging.

When the evidence is inconclusive, record the competing explanations and identify the most likely sequence. For example, one file might be the original March 10 release while another represents a corrected upload from March 12. Make clear when this is your interpretation rather than a documented fact.

## Record confidence and uncertainty

Use the confidence classifications established in Chapter 6 to distinguish established facts from interpretations and speculation:

- Confirmed: Directly supported by reliable surviving evidence.
- Probable: Supported by evidence, but some details remain uncertain.
- Unverified: A reference or claim has been found but not independently confirmed.
- Speculative: A possibility or research hypothesis.
- Unknown: Insufficient information to make a determination.

These classifications are qualitative descriptions of the available evidence, not formal statistical probabilities.

Apply them to individual claims rather than assigning a single confidence level to an entire release.

For example, you might have confirmed where a ZIP file was recovered, consider its identification as version 1.2 probable, but remain uncertain whether it contains the complete original distribution.

Record the evidence behind important conclusions so that another researcher can understand how you reached them.

## Preserve original files and derived copies

One of the most important archival principles is to preserve recovered files independently of anything you create or modify.

You may need to repair an archive, extract an executable installer, repackage files from a CD or rename a file to distinguish it from another recovered copy.

Keep the original recovered file unchanged in `bin/`, and use clear suffixes to distinguish derived versions.

For example:

```
actionq2.zip
actionq2_repack.zip
actionq2_repaired.zip
actionq2_extracted/
```

The names communicate different things:

- `actionq2.zip` is the original recovered archive.
- `actionq2_repack.zip` is an archive recreated from extracted files.
- `actionq2_repaired.zip` is a modified version intended to repair a problem with the original.
- `actionq2_extracted/` contains files extracted from the archive.

If you recover multiple versions of the same original filename, use additional suffixes to distinguish them.

Document every transformation in `history.md`, including the source file, the operation performed and the resulting filename.

Calculate hashes for both the original and derived files. This makes it possible to identify exactly which artefacts were recovered and which were created during the archival process.

The goal is to preserve the original evidence while making useful derived material available to researchers.

## Revisit the release chronology

Verification and classification should lead you back to the historical record.

By now, you may have accumulated enough evidence to revise your understanding of the modification's release history.

Open `research/history.md` and revisit the `Releases and Chronology` section.

Check whether:

- Every known release has a corresponding entry.
- Recovered files are connected to the correct releases.
- Multiple distributions of the same release are distinguished.
- Duplicate files are identified.
- Missing releases or possible intermediate versions are recorded.
- Release dates are supported by evidence.
- Conflicting dates and uncertain conclusions are documented.
- Patches and supplementary files are distinguished from complete releases.
- Original and derived artefacts are clearly identified.

Update the chronology to reflect new evidence, retaining earlier interpretations where they help explain how your understanding changed. The objective is an accurate and defensible historical record, not one that appears more certain than the evidence allows.

## Keep the README.md up to date

While `research/history.md` is your detailed working historical record, `README.md` is the public face of your archive. It is likely to be the first page most visitors see, and many visitors will come specifically to find and download a copy of the modification.

Include a release list with the best available version numbers and estimated release dates. Link each recovered release directly to its corresponding file in `bin/`, so visitors can easily find and download it.

For example:

```
## Releases

| Version | Date | Download |
|---|---|---|
| 1.0 | 1997-04-12 | [actionq2.zip](bin/actionq2.zip) |
| 1.1 | 1997-06-?? | [actionq2_11.zip](bin/actionq2_11.zip) |
| 1.2 | ? | actionq2_12.zip |
| 1.3 | ? | ? |
```

Use your best estimates when exact dates or version numbers are unknown. Use `?` for information you cannot establish. If you know a file existed but have not yet recovered it, include its original filename without a download link. This makes missing material visible and helps other researchers understand what is still being sought.

You can also distinguish between complete releases, incremental patches, beta versions and other supplementary files. Where multiple distributions of the same version exist, make the distinction clear rather than presenting them as separate official releases.

The README should not reproduce all the evidence and uncertainty discussed in `history.md`. Its purpose is to communicate the clearest and most useful summary you can currently provide. Link to the detailed historical record for readers who want to understand the evidence behind the chronology.

Remember that the README is a living document. As you recover additional files, resolve uncertainties and revise your understanding of the release history, update it accordingly. The public archive should always reflect your best current understanding, even when that understanding is incomplete.

## Chapter summary

Recovering files is only part of archival research. Each discovery needs to be examined, verified, classified and connected to the historical record.

The result is more than a collection of downloads. It is a documented account of what has survived, how the recovered artefacts relate to the original releases and what remains uncertain.

**Outcome:** You can turn recovered material into a coherent and defensible archival record.

With your recovered files verified, classified and connected to the historical record, you are ready to share the results of your work. The next chapter explains how to publish your archive so that others can explore its history, download the recovered files and help fill the remaining gaps.
