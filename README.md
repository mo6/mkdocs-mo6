# mkdocs-mo6

A MkDocs theme, derived from the MkDocs [Bootswatch](https://bootswatch.com/) spacelab theme, which in turn is based on [Bootstrap](http://getbootstrap.com/).
The theme is targeted for use in general websites, other than specialised *documentation sites*.
For this goal a couple of extra configuration options are made available, specific for the handling of the sidebar usage (TOC block).

## Usage

To use this theme with your MkDocs project, download/clone in a subdirectory `mkdocs-mo6` and add the following to your `mkdocs.yml` file:

	theme_dir: 'mkdocs-mo6'

## Modifications

The following changes / additions are made compared to spacelab:

- The sidebar (TOC) is moved to the right
- The TOC is not shown on small screens (<= 995px)
- Padding has been added to the bottom of the page
- Page titles are displayed more prominently
- The theme respects the `include_next_prev: False` setting in mkdocs.yml
- The 'Documentation built with MkDocs.' footer message has been removed by default, but can be enabled by the `mkdocs_footer` setting (see below).
- Additional configuration options are added

## Extra mkdocs.yml configuration options

The following configuration options are available for the `mkdocs.yml` `extra` section:

- `min_toc_links: <num>` defines the minimum TOC links needed for the TOC to be displayed. With this option small pages with a few sections don't show a TOC.
- `mkdocs_footer: <boolean>` switches the display of the standard MkDocs footer.
- `build_date_footer: <boolean>` switches the display of the date of the last build.

### Usage

A example use of the options for `mkdocs.yml` is:

```
extra:
    min_toc_links: 2
    mkdocs_footer: true
    build_date_footer: true
```

## Extra page specific meta options

The following meta configurations are available, used to configure individual pages:

- `notoc`: if set it will disable the display of the TOC
- `fullwidth`: if set the page content will fill the whole width of the browser (grid) view
- `showsitemap`: if set it will include a sitemap below the content on the page

### Usage

An example of the use of the meta options in a specific page is:

```
notoc: true
fullwidth: true
showsitemap: true

<div class="jumbotron"><div class="container">
  <h1>Hello, world!</h1>
  <p>...</p>
  <p><a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a></p>
</div></div>

# Hello world

An paragraph of example text.
```

## License

Code released under the [MIT License](https://github.com/mo6/mkdocs-mo6/blob/master/LICENSE).
