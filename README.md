## Overview

The plugin allows preparing your text for publishing by correcting typography. It helps to automatically place non-breaking spaces, remove extra spaces, correct minor typos, insert correct quotes, replace hyphens with dashes, and much more.

The plugin is based on [JavaScript Typograf](https://github.com/typograf/typograf). 

Supported languages are listed [here](https://github.com/typograf/typograf/blob/dev/docs/LOCALES.en-US.md).

Typograf is compatible with [self-hosted](https://github.com/ONLYOFFICE/DocumentServer) and [desktop](https://github.com/ONLYOFFICE/DesktopEditors) versions of ONLYOFFICE editors. It can be added to ONLYOFFICE instances manually. 

## How to use

1. Choose the locale and the rules you want to apply to your document.
2. Select the text you want to correct.
3. Click the Correct text button.

## How to install

Detailed instructions can be found in [ONLYOFFICE API documentation](https://api.onlyoffice.com/plugin/installation).

## Known issues

* When using the plugin on a document abstract with graphic objects, those objects (images, shapes, Text Arts, tables, charts) are lost. If the shape or other object, contained any text, it will be inserted into the document. Chart legends, titles, etc will be lost.
* Graphic formulas are converted to strings.
* Drop caps, content controls, hyperlinks, underlays, footnotes, bookmarks, caption, tables of contents are removed.
* If at least part of the text is split into columns, then the columns will be applied to the entire document.
* Breaks are not saved.
* Changes suggested using Track Changes are not saved.
* If the plugin is used with Track Changes mode on, the corrected text will be inserted as a suggested change.
* Comments are not saved, except for comments to the whole document.
* Headers and footers remain unchanged if the entire document is selected.
* If header/footer content is selected, graphic objects it contained are lost.
* Line numbering is saved if it is applied to the entire document. If it was applied to a section, then it will be lost along with the section.

## User feedback and support

To ask questions and share feedback, use Issues in this repository.
