# Bookmarklet Compiler
A HTML document/application to create bookmarklets.

You can try it out [here](http://htmlpreview.github.io/?https://github.com/RedAndBlueEraser/bookmarklet-compiler/blob/master/index.min.html).

## Synopsis
This HTML application transforms JavaScript code to bookmarklets.

It carries out a very simple and straightforward transformation, and it is intended as a small fast solution into creating bookmarklets. As a result, it is a single tiny HTML document with embedded CSS and JavaScript. The HTML document can be copied offline and opened as a local file instead of being opened online.

It does not handle any validation of JavaScript code, nor does the whitespace collapsing option take into account of strings or regular expressions.

## Usage

Copy your JavaScript code to be transformed into the first text box.

Choose the options under the Bookmarklet heading.
- `Collapse whitespace`: Collapse all whitespace into one space to reduce the size of the converted bookmarklet. **This also collapses whitespace inside strings and regular expressions.**
- `Wrap in anonymous function`: Wrap the JavaScript code inside an anonymous function. This stops the converted bookmarklet from loading a new page of the JavaScript code.
- `URI-encode specific characters`: Percent-encode specific characters ((Space), ", #, %, &, <, >, ?, @) so the converted bookmarklet contains fewer URI reserved characters. This is usually not required, but kept on as a convention. It can increase the size of the converted bookmarklet.

Get your bookmarklet either by copying the transformed code from the second text box and adding it as a bookmark manually, or simply dragging the link at the bottom of the HTML document to your bookmarks.

## Warnings
- JavaScript code is not validated and the bookmarklet will be created regardless of whether your code is valid or not. Make sure you enter valid JavaScript code.
- `Collapse whitespace` collapses all whitespace in the input including whitespace inside strings and regular expressions. If you want a more comprehensive minifier or obfuscater, process your input through a proper minifier or obfuscater first, such as UglifyJS, before processing it here.

## Author
RedAndBlueEraser
