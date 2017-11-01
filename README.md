# Global LCB - Translations of Little Cree Books stories into other languages

## Overview

The goal of this project is to translate the freely-licensed materials created by [Little Cree Books](http://littlecreebooks.com/) into all of the world's languages so that children and language learners everywhere can enjoy these wonderful stories and create new ones in the same spirit.

All languages are welcome, although translations into Indigenous languages (particularly Cree) should probably be directed to the [Little Cree Books](http://littlecreebooks.com/) main site rather than here. We are particularly interested in translations into languages that have very few resources for early childhood learning. For example, if you are involved in indigenous language revitalization, minority language education, or heritage language learning, we would love it if you could participate in the project.

## Structure

Each top level folder represents a language, identified by its [ISO 639-1](http://en.wikipedia.org/wiki/ISO_639-1) or [ISO 639-3](http://en.wikipedia.org/wiki/ISO_639-3) code, with a preference for the ISO 639-1 "Alpha-2 code", if it exists. For major languages, this code is usually two characters long (e.g., `es`, `zh`, `ar`), although some languages may have three characters (e.g., `yue`).

Within each folder, files are grouped by _story number_ (a four-digit index number that unambiguously identifies the story within the collection). The _basename_ for each story consists of the _story number_ followed by an underscore (`_`), and then the translated name of the story in lower case with any spaces replaced by dashes (`-`).

All of the source files in the repository are stored in Markdown format, and consist of the _basename_ plus the Markdown extension `.md`. Alternate, binary and other formats generated from the source files are named with the _basename_ followed by the appropriate format extenstion.

A list of "core" translateable stories by index number can be found [here](https://github.com/global-asp/lcb-source#stories). The list includes links back to the original versions of each story on the [Little Cree Books](http://littlecreebooks.com/) website.

The stories have been assigned a (random) index number to facilitate the process of linking each canonical story ID with all of the translations available for that story.

## Format

The extracted source text of all stories has been provided here in Markdown format. See [here](https://github.com/global-asp/global-asp#source-format) for specific details about the format used.

A sequence of two hashes `##` on a separate line indicates a page break.

The last section of each story file contains attribution and license information.


There are a few conventions that are used in addition to basic Markdown formatting to allow the files to be easily converted to other formats.

### Story title

The title of the story is indicated at the top (first line) of the Markdown file, following a single hash/pound character and a space (`# `). The title should be on a single line (without linebreaks). If there is a sub-title or other information about the story that should be on the front page (aside from the author name -- see the [Metadata section](#metadata) below), it can be included on lines following the title (but __not__ preceded by a `#`).

### Page breaks

Page breaks within the story are indicated by two `##` characters on a separate line, followed by the text of the following page.

### Sections

For the purposes of this project, stories are conceived of as individual pages consisting of a single image and accompanying text, with surrounding front and back covers and associated metadata. Though some longer source stories may not conform to this format, it has nevertheless been followed here strictly, in order to make generation of other formats easier.

Sections are defined as the content found between page break markers (`##`), or between a page break marker and the beginning/end of the file.

The first section is roughly equivalent to the cover page and should only contain the title of the story and (in rare cases) a sub-title or other explanatory text that should go underneath the title on the cover. Metadata such as the author name and language of the story will be automatically included when storybooks are generated and should __not__ be in the first section.

The last section is equivalent to the final page or back cover of the storybook, and contains relevant [metadata](#metadata) about the story. See the [Metadata section](#metadata) below for details about what to include here.

### Images

Images from the [LCB Imagebank](https://github.com/global-asp/lcb-imagebank) are automatically included in the generated binary formats and are __not__ indicated in the markup. There is no need to create image links or link to image urls or filenames within the Markdown source.

### Metadata

Story metadata is included in the [last section](#sections) of the Markdown source file.

The metadata section should include the following information:

* License
* Author
* Illustrator
* Translator
* Level
* Language

These should each be on a separate line, and each item of metadata should not be more than a single line. The sections should be kept as consistent as possible. Any additional fields or information other than that listed below will be removed from the generated storybooks.

The metadata section should look something like this:

    * License: [CC BY-NC-SA]
    * Text: Caylie Gnyra
    * Illustration: Caylie Gnyra
    * Translation: Parismita
    * Level: Level 1
    * Language: zh

Notes:
* The License information should always be `[CC BY-NC-SA]` in accordance with the license under which the original stories have been released
* The Translation field should indicate your name rather than the name of the person who translated the original LCB story (if the original that you are working from is a translated story)
* The Language field should exclusively use the appropriate language code for the language you are translating __into__

## Contributing

All contributions are welcome! (This includes reporting issues.)

For the time being, please submit any translations in Markdown format to this repository as pull requests.

Here are some other ideas for ways to get involved:

- Start a new language subfolder for a language we don't have yet
- Proofread / correct errors in existing stories
- Create a new translation of a story
- Record audio for stories that don't have any
- Create a new adaptation/remix of a story in the project (these can be linked to in the wiki)

You can also send .md or plain text files to globalafricanstorybook@gmail.com with your translation or correction and they will be included in the project with attribution. (Please make sure to note "Little Cree Books" in the subject line.)

## About Little Cree Books

> The [Little Cree Books](http://littlecreebooks.com/) above are the first in what we hope will become a large collection of online books designed for early Cree readers. Please check out the [About the Project](http://littlecreebooks.com/about-the-project/) section of this website to learn more about how we hope to develop this collection. The books are currently only available in the Plains Cree dialect, but we hope to offer them in a variety of other dialects as soon as we can. We hope that educators and parents will make liberal use of these resources. Please display them on your classroom SMARTboards, print and/or photocopy them for your students/children, encourage children to read them online, or use them in other creative ways. We simply ask that users do not sell the books. Creative Commons copyright licensing [CC BY-NC-SA](http://creativecommons.org/licenses/by-nc-sa/3.0/) applies to all of the books, unless otherwise noted. Click [here](http://foter.com/blog/files//2012/11/Foter.com_infographic_CC.jpg) for more information on Creative Commons licensing.

## Links

* [nehiyawasinahikanisa](http://littlecreebooks.com/) (Little Cree Books) where you can download the original PDFs of these stories
* [LCB Source](https://github.com/global-asp/lcb-source) - Source text of the Little Cree Books stories in Markdown format
* [LCB Imagebank](https://github.com/global-asp/lcb-imagebank) - A repository containing all the freely-licensed images that accompany these texts

## License

All stories in this repository have been released under a [CC BY-NC-SA](http://creativecommons.org/licenses/by-nc-sa/3.0/) license, allowing them to be shared and modified freely for non-commercial purposes.
