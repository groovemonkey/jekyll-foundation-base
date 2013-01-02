# Jekyll + Foundation CSS #

I love Zurb's Foundation framework, and Jekyll is a great tool for preventing code duplication while building static HTML/CSS/js websites.

This tool really just exists to create a "base" directory for starting new projects.

## What's Included: ##
* all the directories that Jekyll needs to compile your static site
* jQuery
* the foundation framework (css/js/images)
* a default html5 template in _layouts
* a default nav bar under _includes
* orbit slideshow js code in _includes, ready to be called on any page
* default index and 404 page, along with 3 other empty pages


## How To Use It ##
Just download the .zip or

	```git clone git://github.com/groovemonkey/jekyll-foundation-base.git```

this baby and get started!

I hope this is useful to someone else as well, it has certainly made me more productive.

Cheers!

-Dave



## Tutorial: ##


### Layouts ###

The easiest way is to use the default layout (HTML5 Boilerplate -- _layouts/default.html). To use a layout, put this at the top of your page:

    ---
    layout: default
    title: YourPageTitleHere
    ---

<h1>Page-Specific HTML Content</h1>
<p>etc...</p>



### Includes ###

If you're planning on reusing a few snippets of code on several pages, DRY (Don't Repeat Yourself)! Create an include HTML file and put it in the _includes/ directory. Kind of like a Rails helper.

To call an include in a page, just write

    {% include yourincludename.html %}


For an example of this, see _layouts/default.html -- I include the nav.html snippet on the default layout, meaning it displays on every page that uses that layout.


Have Fun!