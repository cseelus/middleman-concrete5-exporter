# middleman-concrete5-exporter

Export your whole sitemap, content and images from your site built with Middleman into a [Starting Point](http://andrewembler.com/posts/concrete5-5.5-content-import-format-sample-content-and-starting/) for [Concrete5](http://www.concrete5.org/).


## Usage

This will create a folder of the same name as this repo inside your *build*-directory, which is the complete **Starting Point** for Concrete5 already. 

1. Drop in this folder (clone it) into your Middlemans *source*-directory
2. Exclude this folder from the page layout by adding `page "/middleman-concrete5-exporter/*", layout: false` to your *config.rb*
3. Run `middleman build`.
4. Copy or link the folder *C5* from inside *build/middleman-concrete5-exporter* into your Concrete5-instance inside the folder *config/install/packages*.

You should really read into [Starting Points](http://andrewembler.com/posts/concrete5-5.5-content-import-format-sample-content-and-starting/) more, if you want to get a glimpse, whats possible

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
