# Start-page generator

Experiment with Jekyll to create a 'start page' to replace your newtab page.

This uses elements from these projects:

 * https://github.com/navigatron/MyStartPage
 * https://github.com/seanvree/homepage

### Issues

This was thrown together quite quickly so some of the CSS stuff overlaps with other bits resulting in a bit of a mess in the final page. So some work needs to be done to make sure each widget doesn't mess with others.


## Configuration

edit `_config.yml` with your desired setup

## Backgrounds

There are three backgrounds available:

 * static-color
 * random-remote
 * day-night

The color for the static background can be set in `_config.yml`

## Widgets

These are the things that get loaded in to the page. More than one can be loaded at once if
needed

There are only 2 right now:

 * navigatron
 * search-ddg


## Building Yourself

There are a number of ways to build your page.

First Install Jekyll then, depending on your needs, run one of these:

### Static build


```shell
bundle exec jekyll build
```

The generated page will be placed in to `_site` with all its supporting files ( css, js, images ).
The contents of this directory could then be placed on a server or just left on your local disk.


### Dynamic build

This may be handy when your developing wigets...

```shell
bundle exec jekyll serve
```
jekyll will update the files as the source files are updated. If you make changes to your config you'll need to stop this process (`^C`) and start it again so the config is re-read.



