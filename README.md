# middleman-concrete5-exporter

Export your whole sitemap, content and images from your site built with Middleman into a [Starting Point](http://andrewembler.com/posts/concrete5-5.5-content-import-format-sample-content-and-starting/) for [Concrete5](http://www.concrete5.org/).


## Usage

Fist, drop in this folder (clone it) into your Middlemans *source*-directory and run `middleman build`.

You'll find a folder of the same name inside your *build*-directory, which is the complete **Starting Point** for Concrete5 already.

It's important to keep the name of this folder -- *c5* -- as it is
connected to the class-name of this Starting Point.


## Check *content.xml* before importing

1. Are the `<page>`'s correctly named?
2. Are the `<page>` pats correct (especially for the homepage)?
3. Do the `<page>` entities contain the content and only the content of the pages you want? 
4. Are the image-paths identical to where you will put your images?
5. Do the `<page>` entities attributes like `description` contain only UTF8 chars?


## To-Do (if possible)
- Get correct order of pages for the page tree, maybe from a pagenav file
