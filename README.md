# mkdocs-mo6

A MkDocs theme, derived from the MkDocs [Bootswatch](https://bootswatch.com/) spacelab theme.

## Modifications

The following changes / additions are made compared to spacelab:

- The sidebar (TOC) is moved to the right
- The TOC is not shown on small screens (<= 995px)
- Padding has been added to the bottom of the page
- Page titles are displayed more prominently
- The theme respects the `include_next_prev: False` setting in mkdocs.yml
- The default 'Documentation built with MkDocs.' message has been removed (sorry)

## Extra mkdocs.yml configuration options

The following configuration options are available for the `mkdocs.yml` `extra` section:

- `min_toc_links: <num>` defines the minimum TOC links needed for the TOC to be displayed. With this option small pages with a few sections don't show a TOC.

### Usage

A example use of the `min_toc_links` option for `mkdocs.yml` is:

```
extra:
    min_toc_links: 2
```
