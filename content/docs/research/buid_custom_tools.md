---
title: 16. Build Tools to Automate Research
weight: 100
---

# 16. Build Tools to Automate Research

Most of the research in this guide can be performed manually using a web browser, search engines, archive websites and file utilities. This is a perfectly reasonable way to begin. However, as an archive grows, some tasks become repetitive and time-consuming. You may find yourself downloading hundreds of historical webpages, searching thousands of files, calculating hashes or comparing directory listings.

This is where small scripts and tools become useful.

This is an advanced topic, primarily intended for readers with some programming experience. You do not need to build software to create a successful Quake archive. However, even a little automation can save considerable time when working with large collections of historical material.

The goal is not to develop a comprehensive archival software system. Instead, build small, reusable tools that perform specific research tasks and produce useful output.

## Start with a repetitive research task

The best automation opportunities usually emerge naturally during research.

For example, you might find yourself repeatedly performing tasks such as:

- Opening hundreds of archived webpages to look for download links.
- Searching historical pages for known filenames.
- Extracting ZIP filenames and directory listings.
- Calculating hashes for recovered files.
- Comparing two versions of a modification.
- Searching a collection of readme files for developer names.
- Building a list of historical download locations.

These tasks are good candidates for automation because they involve repetitive operations that follow predictable rules.

Start by identifying one specific task that takes too much time. Describe what information you have, what you want to discover and what output would be useful.

For example, you might want a script that takes a directory of downloaded HTML pages and produces a list of every ZIP file linked from those pages. This is a relatively small task that can be completed with a short Python script.

Avoid trying to automate the entire research process at once. Build one useful tool, use it during your research, and extend it when another need becomes apparent.

## Choose a simple programming language

Python is a good choice for archival research tools. It is relatively easy to learn, works across Windows, macOS and Linux, and has libraries for working with websites, HTML, compressed files, text documents and cryptographic hashes.

Useful Python libraries include:

- `requests` for downloading webpages and communicating with web services.
- `beautifulsoup4` for parsing HTML and extracting links and text.
- `zipfile` for inspecting ZIP archives and extracting directory listings.
- `hashlib` for calculating MD5 and SHA-256 hashes.
- `pathlib` for working with files and directories.
- `re` for searching text using regular expressions.
- `csv` and `json` for writing structured research results.

You do not need to learn all these libraries before starting. Learn the parts relevant to the task you want to automate.

Python also has a large ecosystem of existing tools and examples. If you encounter a problem, there is a good chance someone has already solved something similar.

## Keep tools small and self-contained

For this type of research, a collection of small scripts is generally more useful than a large application.

A simple structure might look like this:

```
action-quake-archive/
    README.md
    bin/
    research/
        tools/
            download_wayback.py
            extract_links.py
            search_pages.py
            inventory_archives.py
            calculate_hashes.py
            compare_releases.py
```

Each script should perform one reasonably well-defined task.

For example:

- `download_wayback.py` retrieves selected archived webpages.
- `extract_links.py` extracts links from downloaded HTML files.
- `search_pages.py` searches downloaded pages for filenames and project names.
- `inventory_archives.py` examines ZIP files and produces file listings.
- `calculate_hashes.py` calculates checksums for recovered files.
- `compare_releases.py` compares the contents of two releases.

Initially, keep each tool in a single Python file. Avoid unnecessary packages, complex project structures, databases and configuration systems.

A tool should be easy to understand, modify and run several months later when you have forgotten how it works.

You can always introduce more structure if a tool becomes sufficiently complicated to justify it.


## Download and search archived websites

One of the most useful automation opportunities is extracting information from historical websites.

The Wayback Machine provides a CDX API that can be used to discover archived URLs for a particular website. A script can query this API, retrieve the resulting URL list and identify pages or downloadable files worth investigating.

A good place to get started with the Wayback Machine's APIs is this website:

* [Wayback Machine APIs](https://archive.org/help/wayback_api.php)\
    `https://archive.org/help/wayback_api.php`

For example, you could build a tool that:

1. Accepts a project website domain.
2. Queries the Wayback Machine CDX API.
3. Retrieves a list of archived URLs.
4. Filters the results for HTML pages, ZIP files and other interesting extensions.
5. Removes duplicate URLs.
6. Writes the results to a text file.

This can quickly produce a useful list of historical pages and download locations.

You can build further tools to process the downloaded HTML pages.

**Extract links from HTML pages**

A project homepage might contain links to news pages, downloads, screenshots, documentation and external mirrors. A script using Beautiful Soup (a Python library mentioned above) can extract all the links from an HTML page and write them to a text file.

**Identify downloadable artefacts**

You can filter extracted links for common archive and file extensions, including:

- `.zip`
- `.rar`
- `.7z`
- `.pak`
- `.pk3`
- `.exe`
- `.dll`
- `.txt`

This helps identify potential release files and supplementary material without manually inspecting every link.

**Search archived website content**

You can search downloaded HTML pages for known filenames, version numbers, developer names and project names. This is particularly useful when you have accumulated many archived pages from different dates.

**Identify external mirrors**

Historical project websites often linked to external FTP servers, personal websites and community hosting services. A script can extract links pointing to external domains and produce a list of potential mirrors to investigate.

The result is a searchable inventory of historical file locations and website references.

There are limitations. The Wayback Machine does not necessarily preserve every page or downloadable file, and an archived page may contain a link to a file that was never captured. Treat extracted links as research leads rather than proof that a file is available.

## Analyse recovered files

As your collection grows, you will accumulate many ZIP archives and other files. Manually inspecting every archive becomes increasingly inefficient.

Small scripts can automate much of this work.

**Calculate file hashes**

A script can recursively examine a directory and calculate MD5 and SHA-256 hashes for every file.

These hashes are useful for identifying identical files, even when they have different filenames or are stored in different directories.

For archival records, SHA-256 is a good default. MD5 can also be useful when comparing files against older catalogues or historical checksum lists.

Write the results to a text file or CSV containing the filename, file size and hashes.

**Identify duplicate files**

Once hashes have been calculated, files with matching hashes can be grouped together.

This is particularly useful when you have recovered the same modification from several different sources. You may have copies from an original website, a magazine CD, an FTP mirror and another community archive.

Rather than assuming that different filenames indicate different releases, compare their contents and hashes.

**Inspect ZIP archives**

Python's `zipfile` library can examine ZIP archives without extracting their contents.

A script can generate a directory listing for each archive, including filenames, file sizes and internal timestamps.

This allows you to compare the contents of recovered releases and identify files that may have been added, removed or renamed.

**Read documentation automatically**

Many modifications contain readme files, installation instructions and changelogs.

A script can identify likely documentation files inside ZIP archives and extract their contents for searching. You can use this to find version numbers, release dates, developer names and other historical information.

Be aware that old readme files may use different text encodings. Some may also be stored in formats that require additional processing.

**Compare different releases**

You can build tools that compare two or more releases of the same modification.

For example, a comparison might identify:

- Files present in one release but missing from another.
- Files that have changed between releases.
- Changes in file sizes.
- Different versions of readme files.
- New maps, models, sounds or other assets.
- Identical files appearing under different names.

These comparisons can help establish whether two recovered archives represent different releases, repackaged versions or simply duplicate copies.

## Create research indexes

Another useful application of automation is building searchable indexes of the material you have already collected.

As research progresses, you may have hundreds of HTML pages, readme files, news articles, Usenet messages and directory listings. Searching these documents individually becomes increasingly inconvenient.

A simple indexing script can search an entire directory of text files and report matching filenames and locations.

For example, you might maintain a list of known filenames and search every downloaded document for references to them. The results could identify:

- Historical download links.
- News articles mentioning a particular release.
- Readme files referring to an earlier version.
- FTP listings containing a known filename.
- References to developers or project contributors.
- Pages that mention a release but use a different project name.

You can also generate indexes of all recovered files, including their filenames, sizes, hashes and containing archives.

The output does not need to be sophisticated. A plain text file or CSV spreadsheet is often sufficient.

The important thing is that the information becomes searchable and can be used to guide further research.

## Keep output simple

The purpose of these tools is to assist research, not create another software project that requires ongoing maintenance.

For most archival tasks, plain text output is sufficient.

For example, a file inventory might contain:

```
actionq2.zip
    Size: 1,245,678 bytes
    SHA-256: ...

actionq2_15.zip
    Size: 1,386,421 bytes
    SHA-256: ...
```

A link extraction tool might produce:

```
https://example.com/downloads/actionq2.zip
ftp://ftp.example.com/pub/quake/actionq2_15.zip
https://mirror.example.net/actionq2/readme.txt
```

A search tool might produce:

```
Search term: actionq2_15.zip

Found in:
    planetquake_news_1998.html
    aq2_project_readme.txt
    ftp_directory_listing.txt
```

You can redirect console output into a text file when you want to preserve the results:

```
python search_pages.py actionq2 > search_results.txt
```

For larger inventories, CSV is useful because the results can be opened in a spreadsheet and sorted or filtered.

Avoid introducing a database or web interface unless you have a specific reason to do so. A text file that you can inspect, search, compare and preserve is often all you need.

## Be considerate when accessing historical servers

Automation makes it easy to send large numbers of requests to websites and download large collections of files. Just because you can automate these operations does not mean you should do so without considering the server.

Some historical websites and FTP archives are maintained by volunteers or operate on limited infrastructure. Excessive requests can place unnecessary load on these services.

When writing tools that access remote servers:

- Introduce a delay between requests.
- Avoid downloading the same page or file repeatedly.
- Cache previously retrieved results where practical.
- Limit the number of requests made in a single run.
- Avoid recursively downloading entire websites or FTP directories without a clear reason.
- Check whether a service provides an API or published access guidelines.
- Stop if a server begins returning errors or appears unable to handle requests.

For example, a script that queries the Wayback Machine should not issue hundreds of requests in rapid succession. Retrieve the information you need, wait between requests and save the results locally.

Prefer targeted research over indiscriminate downloading. If you know the likely release filenames or the relevant period of a website, use that information to narrow your searches.

## Use AI to help build research tools

You do not need to be an experienced programmer to benefit from automation. Modern large language models can help you write small scripts based on plain-language requirements.

This is particularly useful for the kinds of focused tools described in this chapter.

You can describe what you want the tool to do, provide examples of input files and explain what output you expect. An AI assistant can generate an initial Python implementation, explain how to run it and help resolve errors.

For example, you might ask:

> Write a Python script that recursively scans a directory for ZIP files. For each archive, extract the filenames, file sizes and internal timestamps without extracting the files. Write the results to a CSV file. Include the archive filename as a column so I can compare different releases.

You can then test the script against a few known archives and ask the assistant to modify it when you encounter problems.

This approach is sometimes called *vibe coding*. You describe the desired behaviour and use an AI assistant to generate and refine the implementation.

However, generated scripts should not be trusted without testing. They can contain bugs, make incorrect assumptions about file formats or accidentally modify files.

A sensible process is to:

1. Describe one specific research task.
2. Provide a small sample of the input data.
3. Specify the expected output.
4. Ask the AI assistant to generate a simple Python script.
5. Run it against a small test collection.
6. Inspect the results manually.
7. Correct any problems before using it on the full archive.

Be especially careful with scripts that rename, move, modify or delete files. For archival work, prefer read-only operations wherever possible. Keep original files untouched and test potentially destructive operations on copies.

AI makes it much easier to build small research tools, even if you only have basic programming knowledge. You still need to understand what the tool is supposed to do and verify that its results are correct.

## Build tools that can be reused

A useful research tool should ideally work across multiple archival projects.

For example, a script that calculates hashes should not be tied specifically to Action Quake 2. It should accept a directory as an input and process whatever files it finds.

Likewise, a tool that extracts links from HTML pages should work with any project website, not just one particular Quake modification.

This is one reason to keep tools generic and configurable. Rather than hardcoding project names, filenames and directory paths into the script, accept them as command-line arguments or simple configuration values.

You can then reuse the same tools when researching a different modification, a different Quake game or even an unrelated software archive.

Over time, you may develop a small personal collection of research scripts that becomes increasingly useful with each new project.

## Chapter summary

Automation is not necessary for creating a Quake archive, but it becomes increasingly valuable as the amount of historical material grows. Small Python scripts can download and search archived websites, extract historical links, analyse recovered files, calculate hashes, compare releases and build searchable research indexes.

Keep tools focused, generic and easy to reuse. Prefer single-file scripts with simple console, text or CSV output rather than developing a large archival application. Use AI assistants to help write and refine scripts, but test their behaviour and verify their results before relying on them.

The aim is to spend less time performing repetitive operations and more time investigating the history, identifying missing releases and improving the archive.

**Outcome:** You can automate repetitive research tasks and process large collections of historical material more efficiently.