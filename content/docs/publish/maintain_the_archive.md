---
title: 19. Maintain and Improve the Archive
weight: 3
---

# 19. Maintain and Improve the Archive

Publishing your archive is an important milestone, but it does not necessarily mean the project is finished.

New files may surface, developers and collectors may provide additional information, and other archivists may identify gaps in your research. Even after you have exhausted the available sources, opportunities for new discoveries may arise months or years later.

An archive should therefore be treated as a living preservation project.

You do not need to work on it continuously. Instead, maintain the archive as new information becomes available and periodically revisit your research with fresh eyes.

The goal is to preserve what you have recovered while allowing the archive to become more complete and accurate over time.

## Accept Contributions from Others

Once your archive is public, other people may contact you with files, information or corrections.

Contributions might come from former developers, players, collectors, researchers or other Quake archivists.

Some people may offer complete releases that are missing from your collection. Others might provide a single screenshot, an old download URL or a recollection about when a particular version was released.

Treat these contributions as new research leads rather than automatically accepting them as established facts.

When someone contributes a file, ask where and approximately when they obtained it. Distinguish original developer distributions, personal backups and copies recovered from third-party collections, recording the provenance alongside the file.

For historical claims, ask whether the contributor has supporting evidence. Personal recollections can provide useful leads, but contemporary records generally offer stronger support for specific dates and events.

Remember to acknowledge contributors and respect their preferences about how they are credited.

## Evaluate Newly Discovered Files

When you receive a new file, do not immediately add it to the public release list.

Apply the techniques from [Chapter 17: Verify, Classify and Connect Discoveries](verify_and_classify_files.md), comparing the new file's hash and contents against the existing collection.

Determine whether it is:

- A previously missing release.
- An alternative distribution of an existing release.
- An identical copy of a file already preserved.
- A patch, update or supplementary download.
- A repackaged or modified copy of an existing release.
- An unidentified file requiring further investigation.

If the file is genuinely new, record its filename, size, hash, contents and provenance in `research/history.md`.

If it is a duplicate, the additional source may still be worth documenting. Independent copies can help establish that a particular distribution was widely available or confirm the identity of a previously uncertain file.

Preserve the original file without modifying its contents.

Only add the file to `bin/` and link it from the README when you have established how it fits into the archive and are satisfied that it is appropriate to redistribute.

If its identity remains uncertain, document the questions and continue investigating.

## Update the Release History

New discoveries may change your understanding of the modification's history. You might recover a previously unknown version, identify an unofficial release or establish a more accurate release date.

Update the `Releases and Chronology` section of `research/history.md` to reflect the new evidence, adding or correcting entries as appropriate.

If recovered files resolve outstanding entries in `research/wishlist.txt` or `research/wishlist_urls.txt`, update those lists as well.

Finally, update the README so that visitors can immediately see which releases are available and how the project's history has changed.

## Correct Historical Information

Historical research is rarely perfect, and new evidence may overturn earlier conclusions.

For example, a date originally identified as a release date might prove to be the date a file was uploaded to a mirror. Correct the release entry, distinguish the two events and document the supporting evidence.

Where a correction is significant, briefly document the reason for the change.

You do not need to maintain a detailed history of every minor edit. Git already records changes to your repository.

However, important corrections to release identities, dates, authorship or provenance deserve an explanation in `research/history.md`.

This helps future researchers understand why the archive presents a particular interpretation.

## Preserve New Evidence

Not every new discovery will be a downloadable modification file.

You may find an archived news article, a previously unknown project website, a forum discussion or an FTP directory listing that provides useful historical information.

Add useful evidence to `research/history.md`, connecting it to the relevant release or historical event. Where appropriate, preserve a local copy and record the original URL, archived URL, publication date and other identifying details.

A forum post or personal website that is accessible today might not remain available indefinitely.

If a source supports an important claim in your historical record, try to preserve enough information that another researcher can understand and verify the claim even if the original website becomes unavailable.

Avoid collecting material without a clear purpose. Focus on evidence that helps establish the modification's history, identify its releases or explain the provenance of recovered files.

## Record Changes to the Archive

Record significant additions and corrections using descriptive Git commit messages.

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

Continue tracking unresolved questions in `research/notes.txt`, missing releases in `research/wishlist.txt` and historical download locations in `research/wishlist_urls.txt`. Revisit these records as new evidence becomes available.

For larger questions, GitHub Issues can also be useful.

An issue can describe a specific problem, such as identifying an unknown release, finding an original ZIP or resolving a conflicting release date.

Other researchers can then contribute information directly to the discussion.

Close issues when they are resolved, but retain the discussion as part of the project's research history.

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

As recommended in [Chapter 18: Publish the Archive](publish_the_archive.md), maintain an independent backup of recovered files, research documents and evidence, preferably on a separate drive or storage service.

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

Read the README and historical record with fresh eyes, looking for gaps in your reasoning, confusing descriptions and unresolved questions. Check for responses to community announcements, review any contributions and investigate promising leads you may have overlooked.

Use this first revisit to tidy the archive and address problems that become apparent after some distance from the original research.

### Revisit after six months

After six months, consider conducting another research pass.

New collections, recovered websites and discoveries made by other archivists may provide opportunities that did not exist during your original investigation.

You may also have discovered new research tools, FTP mirrors, CD collections or search techniques while working on other projects.

Apply these resources to your earlier archive, focusing on missing releases and promising unresolved leads.

You do not need to repeat every search from the beginning. Focus on opportunities that were not available or not considered during your first investigation.

### Revisit after one year

After a year, conduct a broader review of the archive.

Consider what you have learned about Quake archiving over the past year. New tools, research techniques, historical sources and connections between projects may allow you to approach the archive with a deeper understanding.

Use this experience to conduct a broader reassessment of the project.

Review the release history, outstanding questions and missing files.

Check whether the archive's documentation remains accurate and whether its external resources are still available.

If the archive is already as complete as you can reasonably make it, there is no need to manufacture more work.

Simply confirm that the collection remains accessible and leave it available for future contributors.

## Understand That Completeness Can Improve Over Time

An archive does not have to be complete to be valuable. Additional releases, source code, development builds and historical evidence may surface months or years after the original research.

Completeness is therefore not a fixed state achieved when the archive is first published. It can improve as new material becomes available.

There may also be different kinds of completeness.

You might recover every known public release but still lack supplementary files, source code or historical documentation.

Alternatively, you might have extensive historical documentation but be missing several original distribution archives.

Your archive can make progress in any of these areas.

Be realistic about what can be achieved.

Some files may be permanently lost, and some historical questions may never be answered.

The purpose of an archive is not to guarantee that every piece of information can be recovered. It is to preserve what survives, document what is known and make future discoveries possible.

## Know When to Stop

Maintaining an archive does not mean working on it indefinitely. When available leads are exhausted and additional research produces little new information, it is reasonable to stop actively searching.

Leave the archive accessible and documented, returning when new opportunities appear or when you feel motivated to investigate again.

You may also choose to begin another archival project.

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

**Outcome:** You can maintain and improve your Quake modification archive over time, incorporating new discoveries and keeping it accurate, accessible and useful.

