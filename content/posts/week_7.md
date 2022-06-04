Title: Week 6 - A full week(ish) to focus on science.
Slug: week_6
Category: weeknotes
Tags: refactoring, documenting
Date: 2022-03-04


Well it didn't quite work out due to urgent family things, but it was lovely to have a couple of days to just focus on this project. I managed to get a significant part of the structure processing pipeline working using the new shared library of functions (these will be shared between several of the different parts of the project and give a consistent access to things like Amazon S3 storage).

At the same time of doing the refactoring, I created a minimal user interface for the structure processing pipeline and also created docstrings and type hints for all the functions. Since I'm doing this part time, these are essential. There was quite a lot of head scratching looking at code which was written a month or longer ago. I've read a few blog posts from a colleague at The Guardian and amazing engineer/maker of things [Simon Willison on using docstrings](https://til.simonwillison.net/sphinx/sphinx-autodoc) and I'm now a big fan of "documentation first" development.

The next phase of work will focus on making sure that datasets on the individual positions within the MHC molecules are consistent across all molecules, regardless of deletions or insertions. This has been quite complex to think through, but I think I now have a scalable solution to the problem.

One problem to be solved is that the current mechanism for aligning structures to each other is very particular about contiguous and identically numbered sequences so another mechanism will need to be found for that. 

### **Papers Read**

https://www.cell.com/cell-reports/fulltext/S2211-1247(22)00239-X
