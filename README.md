# Zotero Obsidian Zettelkasten

This repository presents my current Zettelkasten workflow based on the use of two softwares : Obsidian and Zotero.

Zettelkasten (german for 'slip box') is a note-taking and personal knowledge management method that is frequently associated with great success in science, research, study and writing (see [Nicklas Luhmann](https://en.wikipedia.org/wiki/Niklas_Luhmann)). Obsidian is a free (but proprietary) _knowledge base/note-taking_ software, while Zotero is a free and open-source reference management software. In other words, Zotero is the software I use to create my digital library of references, articles and books (basically a bank of .pdf and .html files) and Obsidian is where I take note, capture thoughts, write ideas and organize everything else.

Many have already presented Zettelkasten workflows similar to what you will find here, and I don't pretend to have created anything original regarding the method of Zettelkasten, Obsidian or Zotero, far from it. As such, I will try and add the references I found and used as they come up and list everything in the [References](#references) section. However, I thought many could use this written guide to set-up the workflow for themselves and I wanted to share the Zotero Custom Import template I use (see [Zotero Integration](#zotero-integration)). Creating this template is not trivial if you are not already familiar with the ins and outs of obsidian or are not willing to do a bit of _coding_ yourself (I consent to use the word _coding_ quite liberally).

## Gallery

### What the workflow looks like in 60 sec.

**LINK TO VIDEO**

Ok, I grant you, it's a bit jarring. I would completely understand for someone that never used Zotero and obsidian to be completely lost. So here are some screenshots of the different steps (more info in the [Workflow](#workflow) section)

### Step 1: Add reference to Zotero

### Step 2: Annotate PDF in Zotero

### Step 3: Import Zotero annotation in Obsidian

## Installation and Set-up

Install the following programs and extensions

### [Zotero](https://www.zotero.org/)

#### Zotero extensions

  - [Zotero browser connector](https://www.zotero.org/download/connectors). This is not *necessary*, but provides a *one-click import* to add references from your web browser directly to Zotero.
  - [Zotfile](http://zotfile.com/). Zotfile is an extension to automatically rename, move and manage PDF attachments. It can be used to configure your library to be located in a cloud synced folder (for instance).
  - [Better bibtex](https://retorque.re/zotero-better-bibtex/installation/). Better bibtex is an extension that makes managing bibliographic data much easier. It is *necessary* for the Obsidian Zotero integration plugin to behave properly.

**Important NOTE** : Trying to download Zotero extensions like zotfile and better bibtex with firefox might not work. This is because Zotero extensions are .xpi files like firefox extensions. To download them, right-click links from their respective download pages and select *save link as...*

Once you downloaded the extensions, launch Zotero and drag-drop the .xpi files to install. You might need to restart Zotero a few times.

### [Obsidian](https://obsidian.md/)

Launch Obsidian and 
#### Zotero Integration

https://github.com/mgmeyers/obsidian-zotero-integration

#### Ad-Monition

https://github.com/valentine195/obsidian-admonition




## Workflow Explanation

### Step 1 : Add references to Zotero.

I use the zotero [browser connector](https://www.zotero.org/download/connectors) to automatically import a reference from any online database ([pubmed](https://pubmed.ncbi.nlm.nih.gov/) in the example). If the .pdf of the reference is openly accessible, zotero will automatically download it and add it to your library. You can also drag and drop any .pdf file inside zotero and it'll grab the metadata if possible.

### Step 2 : Annotate document in Zotero.

I read and annotate pdf documents directly in Zotero. There are 3 possible annotation types: _higlight text_, _sticky notes_ and _select area_. _Highlight text_ are to extract a verbatim portion of the document, _sticky notes_ are to add your own comments somewhere in the document and _select area_ are best suited to capture a figure or part of the document as an image. It is also possible to add comments to _highlights_ and _areas_. All annotations can be searched for in your Zotero library.

### Step 3 : Import Zotero annotations in Obsidian

## References

### Obsidian

#### Youtube

- Nick Milo's [Obsidian for Beginners](https://youtube.com/playlist?list=PL3NaIVgSlAVLHty1-NuvPa9V0b0UwbzBd) series.
  - Start here, great barebone obsidian tutorial. No/Minimal plugin use.
- FromSergio's [Mastering Obsidian](https://youtube.com/playlist?list=PL7oLu8NfQd84_gsyqBVSVgUmCCgcvSZMx) series.
  - This series of video goes into much more details than Nick Milo's one, but is also much longer. There are demos and tutorials for many popular and powerful Obsidian plugins.

### [Zettelkasten](https://en.wikipedia.org/wiki/Zettelkasten)

#### Youtube

- Martin Adams' [Zettelkasten Note-Taking: What I wish I knew about Smart Notes](https://youtu.be/yqKspwjXu18) video.
  - This is where I first learned about Zettelkasten.
- Martin Adams' [Zettelkasten Smart Notes: Step by Step with Obsidian](https://youtu.be/ziE6UExsOrs) video
- Morganeua's [The FUN and EFFICIENT note-taking system I use in my PhD](https://youtu.be/L9SLlxaEEXY) video

#### Book

- Sönke Ahrens [How to take smart notes](https://www.soenkeahrens.de/en/takesmartnotes)
