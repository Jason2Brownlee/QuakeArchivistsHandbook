---
title: 19. Maintain and Improve the Archive
weight: 3
---

# 19. Maintain and Improve the Archive

Publishing your archive is an important milestone, but it does not necessarily mean the project is finished.

New files may be discovered, original developers may provide additional information and other archivists may identify errors or gaps in your research.

Even if you have exhausted every available source, new opportunities may appear months or years later. A previously unavailable website might be recovered, another collector might publish their files or someone might discover an old backup containing a missing release.

An archive should therefore be treated as a living preservation project.

You do not need to work on it continuously. Instead, maintain the archive as new information becomes available and periodically revisit your research with fresh eyes.

The goal is to preserve what you have recovered while allowing the archive to become more complete and accurate over time.

## Accept Contributions from Others

Once your archive is public, other people may contact you with files, information or corrections.

Contributions might come from former developers, players, collectors, researchers or other Quake archivists.

Some people may offer complete releases that are missing from your collection. Others might provide a single screenshot, an old download URL or a recollection about when a particular version was released.

Treat these contributions as new research leads rather than automatically accepting them as established facts.

When someone provides a file, try to establish where it came from.

Ask whether they downloaded it from the original project website, recovered it from an old CD, copied it from another archive or received it directly from a developer.

If they know approximately when they obtained the file, record that information as well.

A file supplied by an original developer may have a different provenance from an identical file recovered from a later compilation CD. Both can be useful, but the distinction is worth preserving.

For historical information, ask whether the contributor has supporting evidence.

A recollection that a modification was released in 1998 may be valuable, but a contemporary announcement or archived website provides stronger evidence for a specific release date.

Remember to acknowledge contributors and respect their preferences about how they are credited.

## Evaluate Newly Discovered Files

When you receive a new file, do not immediately add it to the public release list.

First, examine it using the verification techniques covered in previous chapters.

Calculate its hash, inspect its contents and compare it with files already in the archive.

Determine whether it is:

- A previously missing release.
- An alternative distribution of an existing release.
- An identical copy of a file already preserved.
- A patch, update or supplementary download.
- A repackaged or modified copy of an existing release.
- An unidentified file requiring further investigation.

A different filename does not necessarily indicate a different release.

Likewise, two files with the same filename may contain different versions or distributions.

If the file is genuinely new, record its filename, size, hash, contents and provenance in `research/history.md`.

If it is a duplicate, the additional source may still be worth documenting. Independent copies can help establish that a particular distribution was widely available or confirm the identity of a previously uncertain file.

Preserve the original file without modifying its contents.

Only add the file to `bin/` and link it from the README when you have established how it fits into the archive and are satisfied that it is appropriate to redistribute.

If its identity remains uncertain, document the questions and continue investigating.

## Update the Release History

New discoveries may change your understanding of the modification's history.

You might recover an earlier version that was previously unknown, discover that two releases were distributed on the same day or find evidence that a supposed official release was actually a community modification.

Update the `Releases and Chronology` section of `research/history.md` to reflect the best available evidence.

This may involve adding a new release entry, correcting an existing entry or revising the relationship between releases.

Keep the chronology consistent with the rest of your research.

If a new release is recovered, check whether it fills an existing gap in `research/wishlist.txt`. If it does, update the wishlist.

Likewise, update `research/wishlist_urls.txt` if a previously missing file has been recovered from one of its historical download locations.

Finally, update the README to reflect the new information.

The public release list should always present your best current understanding of the modification's release history.

Visitors should not need to read the detailed research documents to discover that a missing release has been recovered.

## Correct Historical Information

Historical research is rarely perfect.

Early conclusions may be based on incomplete evidence, ambiguous filenames, unreliable timestamps or assumptions that seemed reasonable at the time.

As new evidence becomes available, you may discover that some of those conclusions were incorrect.

Correct the archival record rather than preserving an interpretation simply because it appeared in an earlier version of your documentation.

For example, you might discover that a date previously identified as a release date was actually the date a file was uploaded to a mirror.

Update the release entry to distinguish the two dates and explain the supporting evidence.

Where a correction is significant, briefly document the reason for the change.

You do not need to maintain a detailed history of every minor edit. Git already records changes to your repository.

However, important corrections to release identities, dates, authorship or provenance deserve an explanation in `research/history.md`.

This helps future researchers understand why the archive presents a particular interpretation.

Be willing to revise conclusions, but avoid replacing one unsupported assumption with another.

When the evidence remains inconclusive, document the uncertainty.

An accurate archive does not need to have an answer to every question.

## Preserve New Evidence

Not every new discovery will be a downloadable modification file.

You may find an archived news article, a previously unknown project website, a forum discussion or an FTP directory listing that provides useful historical information.

Preserve this evidence using the same approach established earlier in the guide.

Add the source and connect it to the relevant release or historical event in `research/history.md`.

Where appropriate, save a local copy in your research directory.

Record the original URL, archived URL, publication date and any other information needed to identify the source.

This is particularly important for evidence found on websites that may disappear.

A forum post or personal website that is accessible today might not remain available indefinitely.

If a source supports an important claim in your historical record, try to preserve enough information that another researcher can understand and verify the claim even if the original website becomes unavailable.

Avoid collecting material without a clear purpose. Focus on evidence that helps establish the modification's history, identify its releases or explain the provenance of recovered files.

## Record Changes to the Archive

As the archive evolves, keep a record of significant additions and corrections.

If you are using GitHub, Git already provides a convenient history of changes through commits.

Use meaningful commit messages that explain what was changed.

For example:

```
Add recovered version 0.9 beta
Correct version 1.1 release date
Document original PlanetQuake download URL
Add developer-provided source code
Update missing releases wishlist
```

For larger updates, include a short explanation in the commit description.

This makes it easier to understand the archive's development and recover earlier information if necessary.

You do not need to maintain a separate changelog for a small archive. Git history is generally sufficient.

However, if the archive becomes large or receives frequent contributions, a `CHANGELOG.md` file may become useful for summarising major discoveries.

Keep the maintenance process proportional to the size of the project.

The purpose of recording changes is to preserve accountability and make the archive easier to understand, not to create unnecessary administrative work.

## Track Outstanding Research Questions

Even after publication, your archive may contain unresolved questions.

You might know that a particular release existed but have no surviving copy. You might have two archives with similar contents but be unable to determine which was distributed first.

You may also have leads that were not worth pursuing during the initial research.

Continue using `research/notes.txt` to record these questions and ideas.

Keep missing files in `research/wishlist.txt` and historical download locations in `research/wishlist_urls.txt`.

When new information becomes available, revisit the relevant entries.

For larger questions, GitHub Issues can also be useful.

An issue can describe a specific problem, such as identifying an unknown release, finding an original ZIP or resolving a conflicting release date.

Other researchers can then contribute information directly to the discussion.

Close issues when they are resolved, but retain the discussion as part of the project's research history.

Do not feel obligated to resolve every outstanding question.

A well-documented uncertainty is preferable to an unsupported conclusion.

## Review External Links and Backups

Over time, some of the external resources referenced by your archive may disappear.

Historical websites may go offline, file hosting services may change their URLs and personal collections may become inaccessible.

Periodically review important external links, particularly those used for downloading files or supporting significant historical claims.

If a link no longer works, investigate whether the resource has moved or whether an archived copy is available through the Wayback Machine.

Update the documentation when you find a replacement.

Do not simply delete a historical URL because it no longer works. Original URLs remain useful evidence and may help locate archived copies.

Distinguish the original location from any replacement or archived location.

Also check that the repository's own download links work correctly.

If you host large files outside GitHub, make sure those files remain available.

### Maintain independent backups

Keep at least one backup of the archive outside its public hosting platform.

A local Git repository is useful, but an additional copy on another drive or storage service provides better protection against accidental loss.

Your backup should include the recovered files, research documents and supporting evidence.

Consider preserving the complete Git repository so that its commit history is retained.

For particularly rare material, verify that backup copies can actually be read and that important files still match their recorded hashes.

The files you have recovered may be difficult or impossible to obtain again.

Protecting them is one of the most important responsibilities of maintaining an archive.

## Revisit the Archive with Fresh Eyes

One of the most effective ways to improve an archive is to leave it alone for a while and return to it later.

During the initial research, you may spend days or weeks searching the same websites, investigating the same filenames and following the same leads.

Eventually, the search can become repetitive and discoveries become less frequent.

At that point, it is reasonable to publish what you have and move on.

Returning later can be surprisingly productive.

You may notice something you overlooked, recognise a connection that was not obvious before or think of an entirely different way to search.

You may also have learned new research techniques while working on other archival projects.

A website or search tool that was unfamiliar during your first investigation might now be part of your regular workflow.

Even without any new resources, approaching the same material with fresh eyes can lead to new discoveries.

### Revisit after one month

About a month after publishing, return to the archive for a short review.

By this point, you have had some distance from the original research.

Read the README and historical record as though you were encountering them for the first time.

Look for gaps in your reasoning, confusing descriptions and unanswered questions that now seem easier to investigate.

Check whether anyone has responded to your community announcements or contributed information through GitHub.

You may also think of new search terms, filename variations or sources that were overlooked during the initial investigation.

This first revisit is often an opportunity to tidy the archive and pursue a few promising leads.

### Revisit after six months

After six months, consider conducting another research pass.

The internet may have changed during this time.

New collections may have appeared on the Internet Archive, other archivists may have published additional files and previously unavailable resources may have become accessible.

You may also have started another Quake archival project and discovered useful websites, FTP mirrors, CD collections or research techniques.

Apply these new resources and techniques to your earlier archive.

Revisit the missing files wishlist and investigate the most promising unresolved leads.

Look again at the known releases and consider whether any gaps suggest alternative filenames or distribution locations.

You do not need to repeat every search from the beginning. Focus on opportunities that were not available or not considered during your first investigation.

### Revisit after one year

After a year, conduct a broader review of the archive.

Consider what you now know about Quake archiving that you did not know when the project began.

Perhaps you have developed better tools for searching historical websites, learned how to investigate CD-ROM collections or discovered new communities of collectors.

You may now recognise connections between modifications, developers, hosting services and distribution archives that were not apparent before.

Use this experience to reassess the project.

Review the release history, outstanding questions and missing files.

Check whether the archive's documentation remains accurate and whether its external resources are still available.

If the archive is already as complete as you can reasonably make it, there is no need to manufacture more work.

Simply confirm that the collection remains accessible and leave it available for future contributors.

## Understand That Completeness Can Improve Over Time

An archive does not have to be complete to be valuable.

You may initially recover only a handful of releases, with several important versions still missing.

Months later, another collector might provide an old CD containing one of those releases.

A year later, a former developer might discover a backup containing source code, development builds or files that were never publicly distributed.

Each discovery improves the archive.

Completeness is therefore not necessarily a fixed state achieved at the end of the initial research.

It is something that can improve over time as additional evidence and material become available.

There may also be different kinds of completeness.

You might recover every known public release but still lack supplementary files, source code or historical documentation.

Alternatively, you might have extensive historical documentation but be missing several original distribution archives.

Your archive can make progress in any of these areas.

Be realistic about what can be achieved.

Some files may be permanently lost, and some historical questions may never be answered.

The purpose of an archive is not to guarantee that every piece of information can be recovered. It is to preserve what survives, document what is known and make future discoveries possible.

## Know When to Stop

Maintaining an archive does not mean working on it indefinitely.

At some point, you may have exhausted the available resources and reached a point where additional research produces little new information.

It is reasonable to stop actively searching.

The archive can remain public, with its recovered files, historical record and outstanding questions available to others.

You can return when a new lead appears or when you feel motivated to investigate again.

You may also decide to start another archival project.

This can be particularly valuable because each project teaches you something new.

You will become more familiar with historical websites, FTP archives, file collections, research tools and the Quake community.

These skills can make your next archive easier to research and may eventually help you improve earlier projects.

Over time, a collection of small archival projects can preserve a substantial amount of Quake history.

The important thing is that the material you have recovered remains accessible, documented and protected.

## Chapter Summary

A published archive is not necessarily a finished archive.

New files, historical evidence and community contributions can improve its completeness and accuracy long after the initial research has ended.

Maintain the archive by evaluating contributions, updating its release history, correcting mistakes, preserving evidence and keeping its public documentation current.

Periodically revisit the project after one month, six months and one year. Fresh eyes, new resources and experience gained from other archival projects may reveal opportunities that were previously overlooked.

There is no requirement to work on an archive continuously or to recover every missing file.

**The outcome of this chapter is an understanding of how to maintain a Quake modification archive as an ongoing preservation project, allowing it to remain useful and improve over time.**
