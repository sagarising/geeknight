# Geek Night Pune

An open forum for geeks to connect, discuss &amp; learn latest ideas, technologies and trends in software development

## Quick Start & Auto Deployment

From the GitHub page, navigate to `content` folder and create/edit a `yyyy-mm.html` file. See [content/example.html](content/example.html) for possible parameters. If you save, the changes are automatically deployed at "yet to decide".

**NOTE:** GitHub's "create/edit file" buttons are very small and hard to find, but they are there (as long as you're logged in and have push rights to this repo).

## Manual Development

We're using [nanoc](//nanoc.ws) for static site generation. Jekyll/Octopress are hard-coded for blogging, while Nanoc is much simpler, doesn't take any assumptions and allows to build whatever type of content (not just blogs).

* Make sure you have RVM installed
* Clone this repo
* Run `bundle install`

To start developing,

* Clone this repository
* Forget about whatever present in the root folder
* Worry only about the `generator` folder
* `cd generator` and do `bundle install`. You'll need RVM + Ruby 2.0
* Make changes (see below folder structure). Mostly you'll be dealing with `generator/content`
* Run `nanoc` to compile the website
* Run `nanoc view` to start a server and browse to `localhost:3000`

For ease, there is a Guardfile. You can run `bundle exec guard`, it will keep watching for changes and re-compile the site whenever any file is changed.


# Folder Structure

* `assets` - contains all assets
* `assets/app.sass` - contains the main stylesheet
* `assets/img/speakers` - contains speaker images
* `content` - content for each geek night
* `layouts` - layouts for default and archive versions
* `Rules` - routing rules
* `gh-pages` - folder containing the generated site

# Folders of interest

* `generator` - this is the main source code, rest are all generated source code that can be ignored
* `generator/assets` - contains all assets
* `generator/assets/app.sass` - contains the main stylesheet
* `generator/assets/img/speakers` - contains speaker images
* `generator/content` - content for each geek night
* `generator/layouts` - layouts for default and archive versions
* `generator/Rules` - routing rules


# Front-End Development

* Pure HTML/CSS/Javascript website. No JQuery.
* Used [HTML5 Boilerplate](//html5boilerplate.com) to generate the skeleton.
* Used [colourlovers.com](//colourlovers.com) for the color swatches.
* Using [SASS](//sass-lang.com) and [Foundation](//foundation.zurb.com) for all the Styling.
* Icon fonts were generated and downloaded from [Fontello](//fontello.com). Only icons from the *Modern Pictogram* set were used for consistency.
