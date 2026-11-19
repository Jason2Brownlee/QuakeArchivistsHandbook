---
title: 18. Publish the Archive
weight: 2
---

# 18. Publish the Archive

After researching the modification, recovering its files and reconstructing its release history, the next step is to make the archive publicly available.

A private collection of files and research notes is useful, but a public archive allows others to benefit from your work. Former players can download their favourite modifications, researchers can investigate their history and other collectors can help recover missing material.

Publishing an archive does not require a complicated website or expensive hosting. A simple GitHub repository containing the recovered files and Markdown documentation is sufficient for most projects.

The goal is to create a public resource that is easy to find, easy to browse and easy for others to contribute to.

## **14.1. Prepare the README**

The `README.md` file is the front door to your archive.

Most visitors will not be interested in the details of your research. They will be nostalgic Quake players who remember a particular modification and want to download a copy, perhaps to play it again after many years.

The README should make this as easy as possible.

As discussed in the previous chapter, the README should already contain an up-to-date list of known releases, including version numbers, approximate dates and links to recovered files.

Before publishing, review the README from the perspective of someone who knows nothing about your archival project.

Make sure it includes:

- **Project description:** A short introduction explaining what the modification is and why it is worth preserving.
- **Archive contents:** A list of known releases, including version numbers, dates and download links where files are available.
- **Historical research:** Links to `research/history.md` and other relevant documents for visitors who want to investigate the modification's history.
- **Known gaps:** A brief explanation of missing releases, incomplete collections and important uncertainties.
- **Credits:** Acknowledgements of the original developers and people who helped recover material.
- **How to help:** Information about missing files and how visitors can contribute.

Keep the README relatively concise. It should be a useful entry point rather than a complete reproduction of your research.

Visitors who want more information can follow links into the `research/` directory.

## **14.2. Publish the Archive on GitHub**

GitHub is the recommended platform for publishing a Quake modification archive.

`https://github.com/`

GitHub provides free hosting for public repositories, displays Markdown files automatically and allows visitors to browse directories and download individual files.

It also provides Git version control, which is particularly valuable for an archival project.

Every committed change is recorded in the repository's history. If you accidentally remove a file, overwrite documentation or make an incorrect change, you can usually recover an earlier committed version.

This makes GitHub a natural fit for an archive that will continue to evolve as new material is discovered.

To publish your archive:

1. Create a GitHub account if you do not already have one.
2. Create a new public repository with a descriptive name, such as `action-quake-archive`.
3. Upload your existing archive directory, including `README.md`, `bin/` and `research/`.
4. Commit the files to the repository.
5. Open the repository in your browser and inspect how it appears to visitors.

You can upload files through the GitHub website or use Git on your computer.

Using Git locally is recommended if you expect to make regular updates, although it is not essential for a small archive.

Once published, your README will automatically appear on the repository's main page.

Your archive will have a permanent public URL that you can share with other Quake enthusiasts.

If you are new to GitHub and git, the GitHub documentation is excellent and a good place to start:

* [GitHub Docs](https://docs.github.com/) (`https://docs.github.com/`)

### **Why Git version control matters**

Git records the evolution of your archive.

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

## **14.3. Organise the Markdown Documentation**

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

Keep this structure when publishing.

The README provides the main navigation, while the research documents contain the detailed information collected during your investigations.

Use relative Markdown links to connect documents.

For example:

```
[Project history](research/history.md)

[Missing files](research/wishlist.txt)

[Historical download URLs](research/wishlist_urls.txt)
```

Relative links work within GitHub and remain useful if someone downloads or clones the repository.

You do not need to link every research document from the README. Link the documents most likely to interest visitors and contributors.

Informal research notes can remain available without being prominently advertised.

The aim is to make the important information discoverable without overwhelming visitors with the details of your working process.

## **14.4. Publish the Recovered Files**

The most important part of the archive is the recovered files themselves.

For a small Quake modification archive, the simplest approach is to include the files directly in the repository's `bin/` directory.

GitHub allows visitors to browse these files and download them individually.

Link directly to each available release from the README.

For example:

```
| Version | Date | Download |
|---|---|---|
| 1.0 | 1997-04-12 | [actionq10.zip](bin/actionq10.zip) |
| 1.1 | 1997-06-15 | [actionq11.zip](bin/actionq11.zip) |
| 1.2 | ? | actionq12.zip |
```

The first two entries link to recovered files. The third identifies a known release that has not yet been recovered.

This provides a simple way for visitors to find exactly the version they want.

Preserve original filenames and file contents whenever possible.

Do not rename historical releases simply to make the archive look more consistent. Original filenames can be valuable historical evidence and may help other collectors identify matching copies.

Likewise, avoid modifying files inside original distribution archives.

If a recovered release must be repackaged, repaired or otherwise reconstructed, clearly identify it as a derived copy and document the changes in the historical record.

### **File size limits**

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

## **14.5. Link Releases to Their Historical Evidence**

The README is primarily for visitors who want to download files.

However, the archive should also make it possible for interested readers to investigate where those files came from and how their history was reconstructed.

This is one of the main differences between a simple file collection and a historical archive.

Each release listed in the README should correspond to an entry in `research/history.md`.

That entry should contain the supporting evidence gathered during research, such as:

- Original release announcements.
- Historical download URLs.
- Archived project websites.
- FTP directory listings.
- Magazine CD references.
- File sizes and hashes.
- Recovery sources and provenance.

You do not need to reproduce all this information in the README.

Instead, provide a prominent link to the project history and allow readers to explore the evidence themselves.

This also helps other researchers verify your conclusions, identify mistakes and contribute new information.

## **14.6. Document Missing Files and Uncertainties**

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

Likewise, be open about uncertainties in the historical record.

If a release date is unknown, use `?` rather than inventing a date. If the identity of a recovered archive is uncertain, explain the uncertainty in `research/history.md`.

An archive becomes more useful when it distinguishes established facts from incomplete or speculative information.

## **14.7. Credit the People Who Helped**

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

Acknowledgements are important because archival work often depends on the generosity of people who have preserved material for decades.

They also demonstrate that the archive is a community effort rather than simply a collection assembled by one person.

## **14.8. Explain How Others Can Help**

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

GitHub Issues is particularly convenient because it is already integrated into the repository.

Visitors can open an issue to report a missing file, identify an error or provide a link to another archive.

These discussions remain publicly accessible and may help future researchers.

However, not everyone has a GitHub account. Providing an email address or another contact method makes it easier for former developers and collectors to reach you.

Keep the invitation friendly and specific.

You want visitors to understand that even a single old ZIP file, screenshot or recollection could be useful.

## **14.9. Make the Archive Discoverable**

Publishing a repository does not guarantee that people will find it.

Search engines may eventually index the repository, but you can help by using clear names and descriptions.

Choose a descriptive repository name that includes the modification's name and, where useful, the game it belongs to.

Add a short GitHub repository description explaining what the archive contains.

Use relevant repository topics, such as `quake`, `quake-mod`, `quake2`, `game-preservation` or `archive`, depending on the project.

Mention alternative project names and common abbreviations in the README when relevant.

These details help people searching for an old modification recognise the archive.

### **Share the archive with the community**

Once the repository is public, share it with relevant Quake communities.

Suitable places may include Quake forums, Discord servers, Reddit communities and other groups interested in historical game modifications.

Rather than simply announcing that you have created an archive, explain what you have recovered and what you are still trying to find.

For example, mention that you have preserved several releases of a modification but are still looking for an early beta or a particular patch.

Include a link to the repository and invite people to check their old backups.

This gives the announcement a practical purpose and encourages community participation.

You may find that sharing the archive leads to additional discoveries, which can then be incorporated into the repository.

Publishing is therefore not necessarily the end of your research. It can become another way to find missing material.

## **14.10. Consider Copyright and Redistribution Permissions**

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

## **14.11. Maintain Backups and the Repository**

Once the archive is published, it needs occasional maintenance.

GitHub is a convenient public host, but it should not be the only place where your archival material exists.

Keep a local copy of the complete repository and maintain at least one additional backup, preferably on a separate drive or storage service.

This is particularly important for rare files that you recovered from sources that may no longer exist.

Git history helps protect against accidental changes, but it does not replace independent backups.

When updating the repository, continue following the practices established in earlier chapters:

- Preserve original recovered files.
- Record the source and provenance of new material.
- Update `research/history.md` when new evidence changes your understanding.
- Keep the README release list and download links current.
- Update the wishlists when files are recovered or new missing releases are identified.
- Acknowledge people who contribute new material.

Periodically check that download links still work, particularly when files are hosted outside GitHub.

You may also receive corrections or contributions through GitHub Issues or other contact methods. Review these and incorporate useful information into the archive.

A public archive does not need constant attention, but occasional maintenance helps keep it useful and trustworthy.

## **14.12. Keep the Archive Simple**

It can be tempting to build a dedicated website, searchable database or elaborate interface for your archive.

For a small collection, this is usually unnecessary.

A GitHub repository with a good README, a `bin/` directory of downloadable files and a collection of Markdown research documents provides almost everything that visitors need.

It is free, easy to maintain and straightforward for other people to browse.

It also avoids creating a custom software system that you must maintain indefinitely.

If your archive eventually grows into a large collection covering hundreds of modifications or thousands of files, you can consider more sophisticated publishing options.

For now, focus on making the recovered material publicly accessible and the historical information easy to understand.

The archive's value comes from the files you have preserved and the research you have documented, not from the complexity of its website.

## **Chapter Summary**

Publishing turns your working archive into a public resource.

A GitHub repository is a practical starting point because it provides free hosting, Markdown rendering, downloadable files and version control.

The README serves as the main entry point, allowing nostalgic players to find and download releases while directing researchers to the supporting historical documentation.

By documenting missing material, acknowledging contributors and explaining how others can help, you also create opportunities for further discoveries.

**The outcome of this chapter is a publicly accessible Quake modification archive that others can browse, download from, research and contribute to.**