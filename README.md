# anthrologue

Website for anthrologue.

Site design based on the excellent
[al-folio](https://github.com/alshedivat/al-folio), and a lab using
the same theme
[website](https://github.com/DecisionLabUCSF/decisionlabucsf.github.io).

## The basics

Everyone in the lab will be able to:
- [Update their profile](#adding-or-updating-a-profile)
- [Update the list of publications](#updating-the-publication-list)

### Adding or updating a profile

Two steps:

### 1. If you don't have one yet, add a picture to /assets/img/

A good size for team member pictures on this site is 311 pixels wide,
in jpeg or png format. Name your picture file as 'your-name.jpg'.

### 2. Add information to your file in /_members/ 

A placeholder file with your name will likely already have been
created, if not you will have to create your own! This should be
called your-name.md.

At the top of the file is a YAML header where you can add information
that will be included on your page e.g. twitter handle, selected
publications. It looks like this:

```
---
layout: member
title: Your Name 
description: # NB this is your position e.g. DPhil candidate
img: your-name.jpg
year_joined: 2015
email: 
twitter_id: # no icon if left blank
orcid_id: # no icon if left blank
selected_publications: [Author_2020, Author-et-al_2020]
pronouns: they/them
````

Links to external sites such as twitter are generated automatically,
and are represented by an icon. You only have to insert your
handle. This is true for all YAML entries that end in '_id'. If you
leave the entry blank no icon will be generated.

If you want to generate selected publications, you should insert them
as shown above. If you need to add publications, [see
below](#updating-the-publication-list).

Underneath the YAML header there is the content, i.e. the text that
you want to appear on your page. This is markdown, so all the usual
styling applies, e.g. *single asterisk* for emphasis (which also
prints bold on this website). See [this
guide](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## Updating the publication list

You can add publications, so that they appear in the publications page
or your personal page. Note for the former these should be outputs
from anthrologue. The basic machinery is bib.

You should get a citation for the publication as a bib entry. This can
be retrieved from the journal website, Google scholar, or similar. You
then paste it into /_bibliography/papers.bib

You should make sure all fields are inserted correctly, keeping an eye
out for capitalisation. A few things to note:

- citation should be labelled as follows:
  Surname_Year/Surname-Surname_Year/Surname-et-al_Year
  
- include an abbr, which should be either 'repro' or 'calleva'

## License

From [al-folio](https://github.com/alshedivat/al-folio):

The theme is available as open source under the terms of the [MIT
License](https://opensource.org/licenses/MIT).

Originally, **al-folio** was based on the [\*folio theme](https://github.com/bogoli/-folio) (published by [Lia Bogoev](http://liabogoev.com) and under the MIT license).
Since then, it got a full re-write of the styles and many additional cool features.
