---
title: Web Engine Examples
permalink: "/webengine-examples/"
nav_order: 3
---

# Web Engine Examples

Here’s a curated collection of examples of how to use the [WWT WebGL Engine]
in your own web projects.

[WWT WebGL Engine]: https://worldwidetelescope.gitbook.io/webgl-engine-reference/

**Note:** *Due to limitations in our web infrastructure, these examples will
  only work if you access them through unencrypted HTTP, not secure HTTPS.
  Please ensure that you are not visiting this site over an HTTPS channel.*

<!-- Note: no newline before the `endfor` -- needed to get the list to HTMLify properly -->
{% for ex in site.data.webengine_examples %}
- [{{ ex.title }}](#{{ ex.title | slugify }}){% endfor %}

Your contributions are more than welcome! If you’d like to add an example,
please submit a pull request against the
[worldwidetelescope.github.io repository] with your addition.

[worldwidetelescope.github.io repository]: https://github.com/WorldWideTelescope/worldwidetelescope.github.io/

{% for ex in site.data.webengine_examples %}

----

## {{ ex.title }}

{{ ex.summary }}

- [View it live in the browser!](./{{ex.id}}/)
- [View the source code on GitHub](https://github.com/WorldWideTelescope/worldwidetelescope.github.io/tree/master/webengine-examples/{{ex.id}}/)

By: [{{ ex.author_name }}](https://github.com/{{ ex.author_github }}).

{% endfor %}
