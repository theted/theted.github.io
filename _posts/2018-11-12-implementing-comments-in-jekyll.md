---
layout: post
title:  "Implementing comments in Jekyll"
date:   2018-11-13 17:37:22 -0600
categories: jekyll update
---

Jekyll (using the default [minima] theme) supports comments using [disqus] out-of-the-box, only some very minor configuration is needed. The following steps explains how to add comments to your Jekyll site.


### Create an account at disqus
Head on over to [disqus] and create an account through the *I want to install Disqus on my site* button. Choose a `shortname`, which is used for identifing your site with disqus. Don't forget to also confirm your email adress.


### Configuration for Jekyll
Specify the shortname used at disqus to your `_config.yml` file:

{% highlight yml %}
disqus:
  shortname: implementator
{% endhighlight %}

Also make sure that an `URL` is defined in the config.yml file:

{% highlight yml %}
url: "http://theted.github.io"
{% endhighlight %}


### That's it!
Comments are now enabled for every blog post on your site!

To disable comments for a single blog post, simply override the default values in the post file.

{% highlight markdown %}
---
comments: false
---
{% endhighlight %}

Note that comments will only be enabled for blog posts by default. To enable comments on a page, simply include the `disqus_comments` template on the page.

{% highlight markdown %}
{% raw %}{%- include disqus_comments.html -%}{% endraw %}
{% endhighlight %}


[disqus]: http://disqus.com
[minima]: https://github.com/jekyll/minima
