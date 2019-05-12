# WWT Web Examples Static Site

This repository contains the sources for the
[WWT Web Examples](http://webhosted.wwt-forum.org/) website, served
statically via [Github Pages](https://pages.github.com/).

The somewhat unusual repository configuration and custom domain are necessary
for us to serve active web content over plain HTTP, which is in turn required
because the WWT web services are not yet HTTPS-enabled. We are working on it!

## Contributing

As you might guess, contributions to this website, and to the AAS WorldWide
Telescope in general, are welcome! See
[the contributors’ guide](https://worldwidetelescope.github.io/contributing/)
for more information. We use a standard workflow with issues and pull
requests.

## Local testing

This site is based on a standard [Jekyll](https://jekyllrb.com/) static site
system. In short, first run

```
bundle install
```

to make sure that the needed tools are installed, then run

```
bundle exec jekyll serve
```

to serve the site locally. For more information, see
[the GitHub documentation](https://help.github.com/en/articles/using-jekyll-as-a-static-site-generator-with-github-pages)
on Jekyll static sites.
