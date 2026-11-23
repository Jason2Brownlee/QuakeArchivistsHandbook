---
title: 18. Publish the Archive
weight: 2
---

# 18. Publish the Archive

After researching the modification, recovering its files and reconstructing its release history, the next step is to make the archive publicly available.

A private collection of files and research notes is useful, but a public archive allows others to benefit from your work. Former players can download their favourite modifications, researchers can investigate their history and other collectors can help recover missing material.

Publishing an archive does not require a complicated website or expensive hosting. A simple GitHub repository containing the recovered files and Markdown documentation is sufficient for most projects.

## Prepare the README

Before publishing, review the `README.md` prepared during the earlier stages of your project. Consider how it will appear to someone visiting the archive for the first time.

Check that the release list agrees with `research/history.md`, that download links point to the correct files and that missing releases are clearly identified. Make sure repackaged or repaired files are distinguishable from original distributions.

Test links to the historical record, wishlists and other supporting documentation. Confirm that credits are accurate and that visitors have a way to contact you or contribute missing material.

Keep the README concise. Someone looking for a particular release should be able to find it quickly, while readers interested in the historical research should have a clear path to the supporting evidence.

## Publish the Archive on GitHub

GitHub is the recommended platform for publishing a Quake modification archive.

* [GitHub](https://github.com/)\
    `https://github.com/`

GitHub provides free hosting for public repositories, displays Markdown files automatically and allows visitors to browse directories and download individual files.

To publish your archive:

1. Create a GitHub account if you do not already have one.
2. Create a new public repository with a descriptive name, such as `action-quake-archive`.
3. Upload the files you have chosen to publish, including `README.md`, `bin/` and the appropriate documentation from `research/`. Keep private working notes and correspondence outside the public repository.
4. Commit the files to the repository.
5. Open the repository in your browser and inspect how it appears to visitors.

You can upload files through the GitHub website or use Git on your computer.

Using Git locally is recommended if you expect to make regular updates, although it is not essential for a small archive.

Once published, your README will automatically appear on the repository's main page.

Your archive will have a permanent public URL that you can share with other Quake enthusiasts.

If you are new to GitHub and git, the GitHub documentation is excellent and a good place to start:

* [GitHub Docs](https://docs.github.com/)\
    `https://docs.github.com/`

### Why Git version control matters

You might initially identify a file as version 1.2, then later discover evidence that it was actually an earlier beta release. You can update the documentation while retaining the history of your previous interpretation.

Likewise, you might recover a better copy of a damaged file or discover an original distribution archive that replaces an earlier repackaged copy.

Git allows you to record these changes without losing track of what happened.

Use descriptive commit messages, such as:

- `Add recovered version 1.2 release`
- `Document original download locations`
- `Correct release date based on Usenet announcement`
- `Add files recovered from magazine CD`
- `Update missing files wishlist`

A repository's history becomes an additional record of the archive's development.

However, Git version control is not a substitute for the historical documentation in `research/history.md`. Git records changes to your repository, not necessarily the original history of the modification.

## Organise the Markdown Documentation

GitHub automatically renders Markdown files as readable web pages.

This means your existing documentation can serve as a simple website without requiring a separate publishing system.

Your archive already has a straightforward structure:

```
action-quake-archive/
    README.md
    bin/
    research/
        history.md
        notes.txt
        wishlist.txt
        wishlist_urls.txt
```

Keep the basic directory structure when publishing, but decide which research documents should be public. Your historical record and missing-file wishlists are useful to visitors and contributors, while informal notes, private correspondence and unverified working material may be better kept outside the public repository. Review each document before publishing it.

Use relative Markdown links to connect documents.

For example:

```
[Project history](research/history.md)

[Missing files](research/wishlist.txt)

[Historical download URLs](research/wishlist_urls.txt)
```

Relative links work within GitHub and remain useful if someone downloads or clones the repository.

You do not need to link every research document from the README. Link the documents most likely to interest visitors and contributors.

Remember that any file committed to a public GitHub repository can be accessed by visitors, even if the README does not link to it. Keep documents that should remain private outside the public repository.

The aim is to make the important information discoverable without overwhelming visitors with the details of your working process.

## Publish the Recovered Files

The most important part of the archive is the recovered files themselves.

For a small Quake modification archive, the simplest approach is to include the files directly in the repository's `bin/` directory.

GitHub allows visitors to browse these files and download them individually.

Make each recovered release downloadable through the links in your README's release table. Keep missing releases listed without download links so that visitors can distinguish available material from files still being sought.

Publish the original recovered files whenever possible, preserving their historical filenames and contents. Clearly identify any repaired or repackaged copies as derived artefacts, following the practices established in the previous chapter.

### File size limits

GitHub is suitable for most Quake modifications because many original releases are relatively small.

However, GitHub has file size restrictions.

For ordinary Git repositories, GitHub warns about files larger than 50 MiB and blocks files larger than 100 MiB. GitHub also recommends keeping repositories relatively small for good performance.

These limits and recommendations can change, so check GitHub's current documentation before uploading large collections.

If your archive contains very large files, such as CD-ROM images or multi-gigabyte collections, consider hosting those files elsewhere.

Possible alternatives include:

- Internet Archive, particularly for historical software collections and CD-ROM images.
- GitHub Releases, for distributing larger downloadable packages within its applicable limits.
- Other suitable file hosting services that permit public redistribution and long-term access.

Keep the documentation in your GitHub repository and link to externally hosted files from the README.

When using external hosting, record the original filename, file size, hash and hosting location in your research documentation.

External links can disappear, so avoid relying on a single hosting service for the only surviving copy of an important file.

## Link Releases to Their Historical Evidence

A historical archive should allow interested visitors to investigate where its files came from and how their release history was reconstructed.

Each release listed in the README should correspond to an entry in `research/history.md`, containing the supporting evidence gathered during research.

Provide a prominent link to the historical record rather than reproducing its contents in the README. This allows other researchers to verify your conclusions, identify mistakes and contribute additional information.

## Document Missing Files and Uncertainties

Do not wait until every release has been recovered before publishing your archive.

In many cases, a complete collection may never be possible.

Publishing an incomplete archive is still valuable, particularly when it documents releases that are known to have existed but can no longer be found.

Make important gaps visible.

The README should briefly identify missing releases and link to your existing wishlists:

```
## Missing Files

Several historical releases have not yet been recovered.

See the [missing files wishlist](research/wishlist.txt)
and the [historical download URL wishlist](research/wishlist_urls.txt).
```

Your wishlists should provide enough information for someone else to recognise a missing file.

For example, a visitor might remember seeing a particular filename on an old CD or discover that they still have a copy on a backup drive.

## Credit the People Who Helped

Quake modifications were often created by individuals or small teams working in their spare time.

Your archive should acknowledge the original developers and contributors wherever their identities are known.

It should also recognise people who helped you recover files or reconstruct the modification's history.

These might include:

- Original developers who shared old releases or unreleased material.
- Collectors who supplied files from personal backups.
- Community members who identified missing versions.
- Archivists who provided access to historical collections.
- Researchers who found announcements, download URLs or other evidence.

Include a credits or acknowledgements section in the README.

You can also provide more specific acknowledgements in `research/history.md`, particularly when documenting the provenance of individual files.

Ask contributors how they would like to be credited. Some may prefer a username, while others may not want their identity published.

Be particularly careful not to publish private email addresses, correspondence or other personal information without permission.

## Explain How Others Can Help

A public archive creates opportunities for further discoveries.

Someone searching for an old Quake modification might find your repository and realise they have a missing release, an original readme, a development build or a collection of files that could help.

Make it easy for them to contact you.

Include a **How to Help** section in the README.

Explain that you are looking for missing releases, original distribution archives, patches, development files, documentation and historical information.

Link directly to `research/wishlist.txt` and `research/wishlist_urls.txt`.

Provide one or more contact methods, such as:

- An email address.
- A social media account.
- GitHub Issues, where visitors can report discoveries, suggest corrections or offer files.

GitHub Issues provides a convenient, public record of discoveries, corrections and contributions. However, also offer an alternative contact method for people without GitHub accounts, particularly former developers and collectors.

Keep the invitation friendly and specific.

You want visitors to understand that even a single old ZIP file, screenshot or recollection could be useful.

## Make the Archive Discoverable

Publishing a repository does not guarantee that people will find it.

Search engines may eventually index the repository, but you can help by using clear names and descriptions.

Choose a descriptive repository name that includes the modification's name and, where useful, the game it belongs to.

Add a short GitHub repository description explaining what the archive contains.

Use relevant repository topics, such as `quake`, `quake-mod`, `quake2`, `game-preservation` or `archive`, depending on the project.

Mention alternative project names and common abbreviations in the README when relevant.

These details help people searching for an old modification recognise the archive.

### Share the archive with the community

Once the repository is public, share it with relevant Quake communities.

Suitable places may include Quake forums, Discord servers, Reddit communities and other groups interested in historical game modifications.

Rather than simply announcing that you have created an archive, explain what you have recovered and what you are still trying to find.

For example, mention that you have preserved several releases of a modification but are still looking for an early beta or a particular patch.

Include a link to the repository and invite people to check their old backups.

This gives the announcement a practical purpose and encourages community participation.

Sharing your archive can lead to new discoveries, making publication another useful part of the preservation process.

## Consider Copyright and Redistribution Permissions

Quake modifications are historical software, but their age does not automatically make them public domain.

Original developers and other rights holders may still own copyright in the code, artwork, audio, documentation and other content.

Some modifications include readmes or licence files that explicitly permit redistribution. Others may have restrictions or provide no clear statement at all.

Before publishing, inspect the available documentation for redistribution conditions.

Where permission is clearly granted, follow the stated requirements.

Where permission is unclear, consider whether you can contact the original developers or rights holders.

Do not assume that a file being freely downloadable in the 1990s automatically grants unrestricted permission to redistribute it today.

Likewise, avoid adding a repository-wide open-source licence that appears to grant rights over third-party files you do not own.

You can distinguish your own documentation and scripts from the historical files being preserved.

If a rights holder contacts you with a legitimate concern, respond respectfully and be prepared to review or remove affected material.

The purpose of the archive is preservation, not claiming ownership of someone else's work.

## Maintain Backups and the Repository

Before publishing your archive, ensure that you have a complete local copy and at least one independent backup of your recovered files and research documentation. GitHub provides convenient hosting and version control, but it should not be your only copy of historically important material.

Publication is also the beginning of an ongoing preservation responsibility. The next chapter explains how to maintain the archive, incorporate new discoveries, review external links, manage contributions and protect your collection with independent backups.

## Keep the Archive Simple

It can be tempting to build a dedicated website, searchable database or elaborate interface for your archive.

For a small collection, a GitHub repository containing downloadable files and Markdown documentation is usually sufficient. It is free, easy to browse and avoids introducing a custom system that must be maintained indefinitely.

If your archive eventually grows into a large collection covering hundreds of modifications or thousands of files, you can consider more sophisticated publishing options.

For now, focus on making the recovered material publicly accessible and the historical information easy to understand.

The archive's value comes from the files you have preserved and the research you have documented, not from the complexity of its website.

## Chapter Summary

Publishing turns your working archive into a public resource.

A GitHub repository is a practical starting point because it provides free hosting, Markdown rendering, downloadable files and version control.

The README serves as the main entry point, allowing nostalgic players to find and download releases while directing researchers to the supporting historical documentation.

By documenting missing material, acknowledging contributors and explaining how others can help, you also create opportunities for further discoveries.

**Outcome:**  You can make your archive publicly accessible so that others can browse, download from, research and contribute to.

The next chapter explains how to maintain and improve your archive over time, incorporate new discoveries and revisit your research as new opportunities arise.

