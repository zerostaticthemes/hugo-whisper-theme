---
title: 'Configuration'
date: 2019-02-11T19:30:08+10:00
draft: false
weight: 4
---

### Homepage meta tags

Often a homepage requires special meta tags such as a meta description or og meta data for twitter, facebook etc. You can configure these values in the `config.toml`

```
// config.toml
[params]
  google_analytics_id=""

  [params.homepage_meta_tags]
    meta_description = "a description of your website."
    meta_og_title = "My Theme"
    meta_og_type = "website"
    meta_og_url = "https://www.mywebsite.com"
    meta_og_image = "https://www.mywebsite.com/images/tn.png"
    meta_og_description = "a description of your website."
    meta_twitter_card = "summary"
    meta_twitter_site = "@mytwitterhandle"
    meta_twitter_creator = "@mytwitterhandle"
```

### Set meta tags on a per template/page basis

You can set meta tags on a per template basis using a block. For example, you might want to write a custom meta description for the `/services` page. You can insert any valid HTML meta data inside the `{{ define "meta_tags }}` block at the top of a template.

```
// layouts/services/list.html
...

{{ define "meta_tags" }}
    <meta name="description" content="We offer a variety of services in the finance industry" />
```
