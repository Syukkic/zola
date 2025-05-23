
+++
title = "Ergo"
description = "A simple blog Theme focused on writing, inspired by svbtle"
template = "theme.html"
date = 2025-03-17T15:01:15Z

[taxonomies]
theme-tags = []

[extra]
created = 2025-03-17T15:01:15Z
updated = 2025-03-17T15:01:15Z
repository = "https://github.com/insipx/Ergo.git"
homepage = "https://github.com/insipx/Ergo"
minimum_version = "0.4.1"
license = "MIT"
demo = "https://ergo.liquidthink.net"

[extra.author]
name = "Andrew Plaza"
homepage = "https://liquidthink.net"
+++        

[ergo LIVE DEMO](http://ergo.liquidthink.net)



![Ergo Screenshot](https://i.imgur.com/l182IYg.jpg)

A light, simple & beautiful Zola theme made with a focus on writing. Inspired by sbvtle and Pixyll.

Like both those web designs, Ergo is a theme that emphasizes content, but still tries to be stylish. Frankly, the design is
most like sbvtle (http://sbvtle.com) but without the clever svbtle Engine, Javascript, community or kudos button (kudos is on the list of additions, though! But then i'll have to use JS...)
If you find that you like all those things, please check out [svbtle](http://svbtle.com); this theme is meant as a lighter (free) alternative,
and ergo's design will most likely diverge more in the future as this theme evolves with me and it's users (if there are any).
This is not meant as a svbtle clone.


Here's a timelapse:
[![Ergo Creation Timelapse](https://img.youtube.com/vi/ogEjvM-v_-s/0.jpg)](https://www.youtube.com/watch?v=ogEjvM-v_-s)


## Installation
Get [Zola](https://www.getzola.org/) and/or follow their guide on [installing a theme](https://www.getzola.org/documentation/themes/installing-and-using-themes/).
Make sure to add `theme = "ergo"` to your `config.toml`

Ergo relies on having `paginate_by` variable set in `content/_index.md`.

#### Check zola version (only 0.11.0+)
Just to double-check to make sure you have the right version. It is not supported to use this theme with a version under 0.11.0.

### how to serve
go into your sites directory, and type `zola serve`. You should see your new site at `localhost:1111`.

### Deployment to Github Pages or Netlify
[Zola](https://www.getzola.org) already has great documentation for deploying to [Netlify](https://www.getzola.org/documentation/deployment/netlify/) or [Github Pages](https://www.getzola.org/documentation/deployment/github-pages/). I won't bore you with a regurgitated explanation.

### Customizing the Theme
All colors used on the site are from `sass/colors.scss`. There's only about 5-6 colors total.
Change them however you like! Feel free to go into theme and edit the colors. However, editing anything other than `sass/colors.scss` is strongly advised against. Continue at your own peril!

#### Theme Options
```toml
# Specify a profile picture to use for the logos in the theme. It can be svg, png, jpg, whatever, just make sure to copy the logo you want and put it in img/${YOUR_PROFILE}.*
# and update your config.toml accordingly
profile = 'profile.svg'

# Description. This is needed for SEO/site metadata purposes
description = "Simple blog theme focused on writing, inspired by svbtle"

# Color themes used by the theme (theme will use ${color_theme}.css file, generated by SASS or SCSS file with the same name). Defaults to ["default"]. User can choose either of them, default theme is the first in list.
color_themes = ["my-awesome-theme", "default"]

[[extra.socials]] # website
icon = "globe"
icon_class = "fas"
display = "code.liquidthink.net"
uri = "https://code.liquidthink.net"

[[extra.socials]] # github
icon = "github"
display = "Insipx"
uri = "https://github.com/Insipx"

[[extra.socials]] # twitter
icon = "twitter"
display = "@liquid_think"
uri = "https://twitter.com/liquid_think"

[[extra.socials]] # email
icon = "envelope"
icon_class = "fas"
display = "say hello"
uri = "mailto:${MY_EMAIL}@cool_domain.com?subject=hi"

[[extra.socials]]
icon = "instagram"
display = "${your_insta}"
uri = "https://instagram.com/${your_insta}"

[[extra.socials]]
icon = "keybase"
display = "${your_keybase}"
uri = "https://keybase.io/${your_keybase}"

[[extra.socials]]
icon = "linkedin"
display = "${your_linkedin}"
uri = "https://www.linkedin.com/in/${your_linkedin}"

[[extra.socials]]
icon = "reddit"
display = "${your_reddit}"
uri = "https://www.reddit.com/u/${your_reddit}"

[[extra.socials]]
icon = "youtube"
display = "${your_youtube_channel_id}"
uri = "https://youtube.com/channel/${your_youtube_channel_id}"

# Whether to use country flags or language code
country_flags = true
```

## Features
  - [x] Pagination
  - [ ] Dynamic Color Schemes
  - [ ] Edit Colors in `config.toml`
  - [x] NoJS
  - [ ] Analytics
  - [x] Comments?
  - [ ] Like button http://kudosplease.com/
  - [ ] categories?
  - [ ] related posts? (would meaningful related posts, or unmeaningful ones, be worth it w/o database?)
  - [ ] user-requested: Open a Issue, or, if you're feeling up to it, a Pull Request

        