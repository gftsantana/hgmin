hgmin is a theme for the [Hugo](http://gohugo.io) static site generator.
It is designed to load fast and still have a lot of features.

## Installation

```bash
cd path/to/my/site/themes
git clone https://github.com/gftsantana/hgmin.git
```

## Configuration

### Basic configuration

The basic parameters you can use to personalize hgmin are:

- `author`
- `description`
- `metaTags`

An example `config.toml`:

```toml
baseurl = "http:\\example.com"
languageCode = "en-uk"
title = "My Example Website"
disqusShortname = "XYW"
theme = "hgmin"

[params]
  author = "Gildo Santana"
  description = "my awesome example website"
  metaTags = "example, examples, exemplification"
```


### Menus

hgmin uses the built-in [Hugo menus system](http://gohugo.io/extras/menus/). It
currently cannot display multi-level menus.

There is a main navigation menu and a footer menu. They are defined in you config
file. An example `config.toml`:

```toml
[[menu.main]]
  name = "about hugo"
  weight = -110
  identifier = "about"
  url = "/about/"
[[menu.main]]
  name = "getting started"
  weight = -100
  identifier = "getting started"
  url = "/getting-started/"
[[menu.footer]]
  name = "pricing"
  weight = -110
  identifier = "pricing"
  url = "/pricing/"
[[menu.footer]]
  name = "work"
  weight = -100
  identifier = "work with us"
  url = "/work-with-us/"
```
