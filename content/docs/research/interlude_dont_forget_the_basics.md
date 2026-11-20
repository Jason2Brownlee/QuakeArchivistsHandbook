---
title: "Interlude: Don't Forget the Basics"
weight: 51
---

# Interlude: Don't Forget the Basics

One thing I've learned from years of researching Quake modifications is that it's surprisingly easy to overlook the obvious.

As an archival project progresses, I tend to spend more and more time searching for missing files.

I maintain a `wishlist.txt` containing files I know existed but haven't yet recovered. I also maintain a `wishlist_urls.txt` containing historical download locations for those files.

Much of my research eventually becomes an exercise in finding more historical URLs to add to that list.

And I can get quite carried away with it.

I'll come up with increasingly elaborate ideas for where to look. I'll write scripts to crawl old websites, download and index magazine CDs, search forgotten FTP mirrors, and extract download links from archived pages.

It's enjoyable detective work, and sometimes these approaches uncover files I would never have found otherwise.

But there's a problem.

**I sometimes get so caught up in finding new places to look that I forget to check the places I've already found.**

I'll have hundreds of historical URLs for missing files, but I haven't actually checked whether some of them are still live or have surviving captures in the Wayback Machine.

Or I'll discover an old file listing containing dozens of previously unknown releases. I'll carefully add the filenames to my wishlist, research their original download locations, and then move on to the next lead.

Only later will I realise that I never performed a simple Google search for those filenames.

I was so focused on the more interesting research that I'd skipped the obvious steps.

This happened often enough that I eventually started writing scripts to check every URL in `wishlist_urls.txt` against the Internet Archive, looking for archived responses with an HTTP 200 status code.

It became a simple sanity check: **are there files sitting in the Wayback Machine that I should have downloaded already?**

Of course, an HTTP 200 response doesn't guarantee that the archived file is valid or complete. But it's a useful way to identify promising locations that deserve immediate attention.

The lesson is one I still have to remind myself of.

It's easy to become focused on the hunt, especially when you're developing new techniques and discovering obscure sources of historical information.

But the goal isn't to collect the longest possible list of dead URLs, build the most sophisticated search scripts, or discover every forgotten FTP server on the internet.

**The goal is to find and preserve the missing files.**

Don't forget the basics.

Before inventing another elaborate way to search, make sure you've thoroughly checked what you've already found.
