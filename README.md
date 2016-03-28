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
- The default 'Documentation built with MkDocs.' message has been removed (sorry)
- Additional configuration options are added

## Extra mkdocs.yml configuration options

The following configuration options are available for the `mkdocs.yml` `extra` section:

- `min_toc_links: <num>` defines the minimum TOC links needed for the TOC to be displayed. With this option small pages with a few sections don't show a TOC.

### Usage

A example use of the `min_toc_links` option for `mkdocs.yml` is:

```
extra:
    min_toc_links: 2
```

## Extra page specific meta options

The following meta configurations are available, used to configure individual pages:

- `notoc`: if set it will disable the display of the TOC
- `fullwidth`: if set the page content will fill the whole width of the browser (grid) view

### Usage

An example of the use of the meta options in a specific page is:

```
notoc: true
fullwidth: true

<div class="jumbotron"><div class="container">
  <h1>Hello, world!</h1>
  <p>...</p>
  <p><a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a></p>
</div></div>

# Hello world

An parapgraph of example text.
```

