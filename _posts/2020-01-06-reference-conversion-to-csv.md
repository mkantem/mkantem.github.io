---
layout: post
title: References exporting guide from Mendeley to a CSV file!
date: 2020-01-06
tags: writing research bibliography 
Description: This post describes a step by step method to export Mendeley references into a CSV file for use in Ms Excel.

---

If I may quote **Therese Fowler** "Some rules are nothing but old habits that people are afraid to change". 
I recently had to break one of my habits which is using LateX for my writing activities. For the need of a paper, I have been working on, 
I used Ms-Word for the entire paper and I came across an issue. In fact, as the article was a systematic mapping, and for the need for data analysis,
I needed to export my references into a CSV file to be used in Ms Excel. 

It was new because I have been used to deal with BibTex databases only. From my online investigations, I did not find any tool that could 
do the trick in a one-step conversion. Let me take you through the steps I have identified to be the most rigorous and robust way to the conversion.
By any chance, if you found yourself reading this article and don't know what LateX is, 
read [this article](https://mkantem.github.io/notes/2017/07/26/latex){:target="_blank" rel="noopener"}
I wrote a while back on the subject.   

I assume that we all use a reference manager ;) I personally use Mendeley, therefore, the steps might be different if you use another one. 

<h3>Step 1: Export from Mendeley to BibTex</h3> 

In Mendeley Desktop 
 * File --- >  Export
 * Save as type --- > BibTex (*.bib) 
 
 <h3>Step 2: Using JabRef</h3>
 
 LaTeX users might be familiar with this tool but if you are not, you can read about it and download it free of charge from [their website](https://www.jabref.org/){:target="_blank" rel="noopener"}.
 Once you have your BibTex file, you have to open it in JabRef
 * File --- >  Open database
 * And select the BibTex file
 
<h3>Step 3: JabRef to CSV</h3>
 
  * File --- >  Export
  * Choose CSV file type (*.csv)
 
 <h3>Step 4: Import your CSV file to Excel</h3>
 
 * Open a new Excel document
 * Go to data tab and click "From Text"
 * Navigate to the CSV file from the opened window and click import
 * Choose "Delimited" from the new window and click "next"
 * Check the box next to "type of Delimiter" (comma)
 * Click Finnish 
 
As you can see from above, it is a bit tedious but I can ensure you that it works perfectly free of errors and it is always better than typing in
our data line by line into Ms-Excel. At this point, according to your data extraction methodology, you can easily add/use the information at your will.

If you come across a tool that could do this in one step, it goes without saying that I want you to let me know! 
If you think this could interest a peer of yours, feel free to share...
