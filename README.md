# middleman-concrete5-exporter

Export your whole sitemap, content and images from your site built with Middleman into a [Starting Point](http://andrewembler.com/posts/concrete5-5.5-content-import-format-sample-content-and-starting/) for [Concrete5](http://www.concrete5.org/).


## Usage

Just move the folder "c5" from this repo into the `source`-folder of
your Middleman site and the next time you execute `middleman build`
you'll find a folder of the same name inside your `build`-directory,
which is the complete Starting Point for Concrete5 already.

It's important to keep the name of this folder -- "c5" -- as it is
connected to the class-name inside controller.php.
