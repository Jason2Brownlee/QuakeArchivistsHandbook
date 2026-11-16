---
title: Search Usenet archives
weight: 3
---

# **Chapter 6. Search Usenet Archives**

In the previous chapters, we used original project websites and gaming news archives to reconstruct the history of a Quake modification. These sources can reveal release announcements, download links, project websites and information about the people involved.

Another valuable source is Usenet.

Usenet discussions can preserve information that is difficult to find elsewhere. Developers announced releases, users discussed problems, people shared download locations, and community members sometimes posted files directly. These conversations can help reconstruct the history of a modification, even when its original website and downloads have disappeared.

This chapter explains how to search Usenet archives and use the information you find to improve your archival record.

## **6.1 What is Usenet?**

Usenet is an early distributed discussion system that predates the modern web. It became widely used during the 1980s and 1990s, providing a way for people around the world to exchange messages in organised discussion groups called *newsgroups*.

Newsgroups covered almost every subject imaginable, including programming, operating systems, games and individual gaming communities.

For example, Quake-related discussions could appear in groups dedicated to Quake, first-person shooters, game development or general computer gaming. A developer might announce a new modification in a Quake group, while players might discuss it in a broader gaming group.

Usenet messages were distributed between servers. A person would post a message to a newsgroup, and participating servers would exchange copies. Other users could read the message and reply. Replies were commonly linked together into conversations called *threads*.

A typical Usenet message could contain:

- The message subject.
- The author’s name and email address.
- The date and time the message was posted.
- The newsgroup where it appeared.
- The message body.
- Links to websites or downloadable files.
- Replies and references to other messages in the discussion.
- A signature or footer added by the author.

Some messages also included binary attachments. These could be files such as ZIP archives, although binary files were often distributed using specialised posting conventions and could be split across multiple messages.

For a Quake archivist, Usenet is valuable because it provides contemporary evidence. Rather than relying on a modern webpage describing an old modification, you can sometimes find a message written by the developer at the time of the release.

## **6.2 Google Groups**

Google Groups (`https://groups.google.com`) is the most useful starting point for searching historical Usenet discussions. Google acquired the Deja News Usenet archive in 2001 and incorporated its collection into Google Groups.

Google Groups provides access to a substantial archive of historical Usenet messages. It allows you to search for terms, browse newsgroups and read individual messages.

The archive is particularly useful for research into the 1990s and early 2000s, when Quake modifications were actively developed and discussed.

A message in Google Groups can preserve several important pieces of information:

- **The original message:** The text written by the person who posted it.
- **The posting date:** When the message was sent, which can help establish a release or announcement date.
- **The author:** Sometimes a real name, username and email address are available.
- **The newsgroup:** The group in which the discussion appeared.
- **The subject:** Often includes the modification name, version number or release announcement.
- **Thread context:** Replies can provide additional information, corrections and discussion.
- **Links:** Messages may point to original project websites, mirrors or downloadable files.
- **Signatures:** Footers sometimes include personal websites, email addresses or other contact information.

Not every message contains all of this information. Some authors used pseudonyms, some email addresses are missing or obscured, and links may no longer work.

Nevertheless, even a short message can provide a useful lead.

For example, a developer might post:

```
Subject: Action Quake 2 version 1.5 released

From: Developer Name
Date: 12 May 1999

The latest version of Action Quake 2 is now available.

You can download it from:
ftp://example.com/pub/action/action15.zip

See the homepage for the changelog:
http://example.invalid/actionquake/
```

This fictional message provides several useful pieces of evidence:

- A possible release date.
- A version number.
- An original download URL.
- A project homepage.
- The identity or username of the person announcing the release.

Each of these details can lead to further research.

## **6.3 Search Google Groups**

Start by visiting Google Groups (`https://groups.google.com`).

Enter the modification's name into the search box. Google Groups searches message subjects and message contents, allowing you to find both formal announcements and less obvious discussions.

Do not assume that the modification was discussed in only one newsgroup. Search broadly first, then investigate relevant groups and threads.

### **Search the modification's name**

Begin with the most obvious name of the project.

For example, if you are researching Action Quake 2, try:

```
Action Quake 2
Action Quake II
ActionQuake2
AQ2
Action Quake
```

These variations matter because people do not always use consistent naming conventions. One developer might write "Action Quake 2", while a player might refer to it as "AQ2".

A search for only the official project name can miss many relevant messages.

### **Search known filenames**

If you have already recovered some releases, search for their filenames.

For example:

```
action15.zip
actionquake15.zip
aq2-1.5.zip
```

A filename can be particularly useful because people often refer to the actual file when asking for help, reporting a download problem or sharing a mirror.

A discussion might reveal that a file was distributed under a different name, or that a particular version was available from a website that no longer exists.

Search for filenames found in contemporary announcements as well as those found in recovered files.

### **Search developer names**

Search for the names and usernames of developers associated with the modification.

A developer might have posted announcements under their own name rather than the project name. They might also have participated in discussions about other projects.

If you find a likely developer account, inspect other messages posted by that account. These may reveal:

- Other modifications they worked on.
- Personal websites.
- Development teams and collaborators.
- Release announcements.
- Explanations of technical changes.
- Links to files and distribution locations.

Be careful when connecting identities. Two people can use the same username, and a name in a message does not necessarily establish that the author was a particular developer. Record the evidence supporting any identification.

### **Search personal websites**

If you discover a developer's personal website, search for its domain name and distinctive parts of its URL.

For example:

```
developer.example.com
example.com/~developer
```

People sometimes included their website in their message signature. Other users might have linked to it when discussing a modification.

These searches can uncover websites that were not mentioned on the official project homepage.

### **Search alternative spellings and naming conventions**

Repeat searches using variations of project names, developer names and filenames.

Consider:

- Spaces versus no spaces.
- Roman numerals versus Arabic numerals.
- Abbreviations and acronyms.
- Old project names.
- Informal community names.
- Version numbers written in different formats.
- Hyphens, underscores and punctuation.

For example, a project might appear as `Action Quake 2`, `Action Quake II`, `ActionQuake2`, or simply `AQ2`.

The goal is to avoid treating one spelling as the only valid name for the project.

### **Search unique filenames inside recovered releases**

This is a useful technique that is easy to overlook.

A recovered modification might contain hundreds of files, including configuration files, scripts, maps, documentation and custom assets. Some filenames may be distinctive enough to locate discussions about the release.

For example, a ZIP archive might contain:

```
aq2_readme.txt
action_config.cfg
teamplay_guide.txt
```

Search for these filenames individually.

A player might have asked a question about one of the files, or a developer might have posted an explanation of its contents. These discussions can identify the release, reveal its purpose or provide additional historical context.

This technique is especially useful when the project name has changed or is difficult to search for.

### **Search for release announcements and distribution messages**

Look for messages containing words and phrases commonly used when distributing software:

```
released
available
download
new version
mirror
update
patch
beta
final
```

Combine these terms with the modification name or a known filename.

For example:

```
"Action Quake 2" released
"AQ2" download
"action15.zip" mirror
```

Developers sometimes announced their own releases on Usenet. They might include a changelog, explain how to install the modification, link to a homepage or list alternative download locations.

Other users might post messages reporting that a release is available from a mirror or asking where they can download it.

These messages can reveal distribution locations that are not recorded in surviving project websites or gaming news archives.

## **6.4 Investigate Threads and Individual Messages**

Finding a relevant search result is only the beginning. Open the message and examine the surrounding discussion.

A single message might contain a useful download URL, but the replies could explain what the file contains, whether it works, which version it replaces or where another mirror can be found.

Read the complete thread where possible.

Pay attention to the following details:

**Original announcement.** Was the message written by a developer, a player or someone distributing a mirror? This affects how you interpret the information.

**Dates.** Record the date of the message, but distinguish it from the actual release date. A developer might announce a release several days after uploading it.

**Version information.** Look for version numbers, patch numbers, beta labels and references to earlier releases.

**Download locations.** Record every original URL, including FTP links. A URL might no longer work, but it can still provide a valuable lead.

**Changelogs.** Developers sometimes included a summary of changes directly in the message. This can help distinguish releases or identify missing versions.

**Signatures and footers.** A developer's signature might contain a personal website, email address or team affiliation.

**Replies.** Other users might identify a mirror, report a broken link, describe a problem or clarify which release they downloaded.

Do not assume that the first message in a thread contains all the useful information. A reply posted weeks later might be the only surviving reference to a particular download.

## **6.5 Search Other Surviving Usenet Archives**

Google Groups is an excellent starting point, but it is not a complete record of Usenet.

Not every message ever posted was retained, and some messages may be missing from Google's collection. Other archives may preserve material that cannot be found through Google Groups.

Search for alternative Usenet archives and investigate any that appear relevant to your topic.

Useful places to look include:

- **Internet Archive:** `https://archive.org/` contains collections of historical Usenet messages and related data. Some collections are available as downloadable files rather than searchable webpages.
- **Historical Usenet archive websites:** Various websites have preserved newsgroup messages and made them searchable through their own interfaces.
- **Community archives:** Older gaming communities sometimes retained Usenet discussions as part of their own historical resources.
- **Personal collections:** Individuals occasionally publish collections of messages or old newsgroup data.

The availability and search functionality of these archives varies. Some provide a convenient web interface, while others require you to download a collection and search the contents locally.

You do not need to understand the technical details of every archive format to benefit from these sources. Start with searchable webpages and use downloadable collections when they offer a promising source of otherwise unavailable information.

When you find a message in an alternative archive, record the archive's URL and any original message identifiers or headers that are available. This makes it easier to locate the same message again and distinguish it from other copies.

## **6.6 Preserve and Record Usenet Evidence**

Usenet messages should be treated as historical evidence, just like original project websites and gaming news articles.

When you find a useful message, record its details in your archival research.

For example, a release entry in `research/history.md` might include:

```
#### Version 1.5

- Release date: 12 May 1999 (announced)
- Announcement: Usenet message posted by Developer Name
- Newsgroup: alt.games.quake2
- Message date: 12 May 1999
- Original download URL: ftp://example.com/pub/action/action15.zip
- Project homepage: http://example.invalid/actionquake/
- Changelog: Summary included in announcement
- Evidence: https://groups.google.com/...
```

You may also quote the Usenet message in full.

The example is fictional, but it illustrates how a Usenet message can be connected directly to a release.

If the message reveals a new download URL that you cannot recover, add it to `research/wishlist_urls.txt`. If it mentions a missing release or filename, add that information to `research/wishlist.txt`.

### **Preserve uncertainty**

Usenet messages are contemporary sources, but they are not automatically correct.

A user might announce a release date based on when they downloaded a file. A mirror operator might upload a file several days after the original release. A discussion might refer to a beta version using an informal name.

Record what the message actually says rather than converting every statement into a confirmed fact.

For example:

- A developer announces that version 1.5 is available on 12 May.
- A user reports downloading version 1.5 on 10 May.
- A mirror operator reports uploading version 1.5 on 14 May.

These are three different events. They may help establish the release timeline, but they should not be treated as interchangeable dates.

Also distinguish between the author of a message and the developer of a modification. A message can be valuable without its author being directly involved in the project.

### **Preserve links and message details**

Where possible, retain a direct link to the message in Google Groups or the alternative archive.

Also record the original newsgroup, subject, date and author. These details are useful if the archive's interface changes or the message becomes difficult to find.

If you can save a copy of the message, preserve it with your other research evidence. Keep the original message content intact and record where it came from.

A screenshot can be useful as supplementary evidence, particularly when a webpage or message is difficult to access consistently. It should not replace the original message URL or other identifying details.

## **6.9 Summary**

Usenet is a valuable historical source for researching Quake modifications. Its messages can preserve contemporary announcements, developer comments, release information, changelogs, download URLs and discussions about files that are no longer available.

Google Groups is the best starting point, but other surviving archives can contain additional material. Search using multiple project names, filenames, developer identities and distinctive terms found in recovered releases.

Most importantly, treat each useful message as evidence. Record its details, preserve its URL and connect it to the relevant release in your archival history.

**Outcome:** You can use Usenet to discover historical announcements, developer information, filenames and distribution locations.

In the next chapter, we will look beyond websites and online discussions to investigate another important source of Quake history: magazine cover CDs and other physical media.
