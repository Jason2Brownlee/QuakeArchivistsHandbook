---
title: 16. Build Tools to Automate Research
weight: 100
---

# 16. Build Tools to Automate Research

Most archival research can be performed manually using browsers, search engines and file utilities. However, as your archive grows, repeatedly downloading webpages, searching files, calculating hashes and comparing releases can become time-consuming.

Small scripts can automate these tasks and make it practical to investigate much larger collections.

This is an optional, advanced topic. You do not need programming experience to begin preserving Quake files, although some familiarity with Python or a willingness to experiment with AI-assisted programming will help.

The goal is to build small, reusable tools for specific research tasks rather than a comprehensive archival software system.

## Start with a repetitive research task

The best automation opportunities usually emerge naturally during research.

Good candidates for automation include extracting links from archived webpages, searching collections of readmes, generating file inventories, calculating hashes and comparing recovered releases.

These tasks are good candidates for automation because they involve repetitive operations that follow predictable rules.

Start by identifying one specific task that takes too much time. Describe what information you have, what you want to discover and what output would be useful.

For example, you might want a script that takes a directory of downloaded HTML pages and produces a list of every ZIP file linked from those pages. This is a relatively small task that can be completed with a short Python script.

Begin with one useful script and expand your collection of tools as new needs emerge.

## Choose a simple programming language

Python is well suited to archival research. It works across Windows, macOS and Linux and includes libraries for processing websites, archives, text files and cryptographic hashes.

Useful Python libraries include:

- `requests` for downloading webpages and communicating with web services.
- `beautifulsoup4` for parsing HTML and extracting links and text.
- `zipfile` for inspecting ZIP archives and extracting directory listings.
- `hashlib` for calculating MD5 and SHA-256 hashes.
- `pathlib` for working with files and directories.
- `re` for searching text using regular expressions.
- `csv` and `json` for writing structured research results.

Start with the libraries needed for your first task, using existing examples and documentation as a guide.

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

Each script performs a specific research task, making it easier to understand, modify and reuse independently.

Start with single-file scripts and introduce packages, databases or more elaborate configuration only when necessary. Aim for tools that remain easy to understand and run months later.

## Download and search archived websites

The Wayback Machine's CDX API can be queried programmatically to discover archived pages and download URLs; [Chapter 22: Advanced Website Research](../advanced_website_research.md) explains how to use it.

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

Use Beautiful Soup to extract links from downloaded HTML pages, including news pages, downloads and external websites.

**Identify downloadable artefacts**

Filter extracted links by extensions such as` .zip`, `.rar`, `.7z`, `.pak`, `.pk3`, `.exe`, `.dll` and `.txt`.

**Search archived website content**

Search downloaded pages for filenames, version numbers, developers and project names across multiple captures.

**Identify external mirrors**

Extract links to external domains to identify historical FTP servers, mirrors and alternative hosting locations.

Treat extracted links as research leads, not proof that the referenced files survive.

## Analyse recovered files

As your collection grows, you will accumulate many ZIP archives and other files. Manually inspecting every archive becomes increasingly inefficient.

Small scripts can automate much of this work.

**Calculate hashes and identify duplicates**

A script can recursively calculate SHA-256 hashes and file sizes, saving the results to a CSV file. Matching hashes identify identical files, even when filenames or directory locations differ.

MD5 can also be useful when comparing recovered files against older catalogues that used it. Prefer SHA-256 for new archival records.

**Inspect ZIP archives**

Python's `zipfile` library can generate inventories of ZIP archives without extracting them. Include internal filenames, sizes and timestamps to support comparisons between releases.

**Read documentation automatically**

Many modifications contain readme files, installation instructions and changelogs.

A script can identify likely documentation files inside ZIP archives and extract their contents for searching. You can use this to find version numbers, release dates, developer names and other historical information.

Be aware that old readme files may use different text encodings. Some may also be stored in formats that require additional processing.

**Compare different releases**

You can build tools that compare two or more releases of the same modification.

A comparison tool can identify added, removed, renamed or modified files between releases, including changes to readmes, maps and other assets.

These comparisons can help establish whether two recovered archives represent different releases, repackaged versions or simply duplicate copies.

## Create research indexes

A research index allows you to search hundreds or thousands of downloaded webpages, readmes, news articles, Usenet messages and directory listings together. For an application to historical FTP listings, see [Chapter 21: Advanced File Archive Research](../advanced_file_archive_research.md).

A simple script can search a directory of text files and report which documents contain a specified term.

For example, you might maintain a list of known filenames and search every downloaded document for references to them. The results could identify:

- Historical download links.
- News articles mentioning a particular release.
- Readme files referring to an earlier version.
- FTP listings containing a known filename.
- References to developers or project contributors.
- Pages that mention a release but use a different project name.

You can also index recovered files by filename, size, hash and containing archive, using plain text or CSV output.

## Keep output simple

The purpose of these tools is to assist research, not create another software project that requires ongoing maintenance.

Simple text output is often sufficient for archival tools. A search script, for example, might report which documents contain a particular filename:

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

## Be considerate when accessing historical servers

Automated requests can place substantial load on historical websites and FTP archives, many of which are maintained by volunteers or operate on limited infrastructure. Design your scripts to minimise unnecessary traffic.

When writing tools that access remote servers:

- Introduce a delay between requests.
- Avoid downloading the same page or file repeatedly.
- Cache previously retrieved results where practical.
- Limit the number of requests made in a single run.
- Avoid recursively downloading entire websites or FTP directories without a clear reason.
- Check whether a service provides an API or published access guidelines.
- Stop if a server begins returning errors or appears unable to handle requests.

Prefer targeted requests based on known filenames, URLs and release periods rather than indiscriminately downloading entire collections.

## Use AI to help build research tools

Modern AI assistants can help you develop small research tools from plain-language requirements. Describe the task, provide examples of input data and specify the expected output. The assistant can generate an initial Python script and help troubleshoot problems.

For example, you might ask:

> Write a Python script that recursively scans a directory for ZIP files. For each archive, extract the filenames, file sizes and internal timestamps without extracting the files. Write the results to a CSV file. Include the archive filename as a column so I can compare different releases.

This AI-assisted approach is sometimes called vibe coding. Generated scripts may contain bugs or make incorrect assumptions, so test them carefully before using them on your archive.

A practical workflow is:

1. Describe one specific research task.
2. Provide a small sample of the input data.
3. Specify the expected output.
4. Ask the AI assistant to generate a simple Python script.
5. Run it against a small test collection.
6. Inspect the results manually.
7. Correct any problems before using it on the full archive.

When requesting a script, specify that it should preserve original files, handle errors gracefully and report its progress. For tools that download large collections, request caching and a way to resume interrupted work. These requirements can save substantial time and prevent accidental damage to your archival materials.

Prefer read-only scripts wherever possible. Test operations that rename, move or delete files on disposable copies, and verify all generated results before relying on them.

## Build tools that can be reused

Design scripts to work across different archival projects. Rather than hardcoding project names, filenames or directory paths, accept them as command-line arguments or simple configuration values.

For example, a file hashing tool should accept any directory, while a link extraction tool should work with any downloaded website. This makes your scripts reusable across different Quake projects and other historical software collections.

## Chapter summary

Small Python scripts can automate repetitive archival research, including searching historical websites, extracting download links, inventorying recovered files, calculating hashes and comparing releases.

Keep tools focused, reusable and easy to maintain. Use simple text or CSV output where practical, and test AI-generated scripts before relying on them.

Automation should reduce time spent on repetitive tasks so you can concentrate on discovering and preserving historical material.

**Outcome:** You can automate repetitive research tasks and process large collections of historical material more efficiently.

