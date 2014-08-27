---

title: Colophon

---

# Anatomy of a Website, Colophon

As rudimentary as it may be, I'm happy to say all content on this website is written and published by me, one Chris Garrett. Always in the first person, rarely devoid of typos.

It occured to me that, as we discontinued the Abstraktion name to become [Beatroot](http://beatroot.com), we'd lose our sense of legacy. In a vain attempt to give the brand ongoing meaning, and with the agreeance of the team, I decided to adopt the moniker personally.

***

## The Design

I designed the website, roughly, with Sketch. While I grew up on Photoshop, I've recently found a more welcoming home with [Sketch](http://bohemiancoding.com/sketch/) and use it religiously for establishing the broad brush strokes of any new piece of work. I'm a minimalist and pragmatist, and wanted this website's design to serve solely as a vehicle for the content, ensuring it is legible and enjoyable. I hope I've achieved that.

Typography is an unhealthy obsession of mine, and while I'd like to have made use of something more daring, I fell back on old habits and opted for Proxima Nova across the website. While DIN used to be my safety blanket for design, Proxima Nova has gradually assumed the comforting mantle of "typographic woolen-wear".

***

## The Build

Simplistic and elegant content management comes courtesy of [Jekyll](http://jekyllrb.com). I initially experimented with Jekyll on an ill-fated Abstraktion portfolio, one of many that failed to launch during our 3 year life span, and more recently used it for the Beatroot website. Having suffered psychological trauma from far too many "big CMS" projects, how could I not love the simple, elegant combination of [Markdown](http://daringfireball.net/projects/markdown/) and [Git](http://github.com) for managing content?

For any frontend development, I favour a mix of HAML, Coffeescript, SASS and Compass. This necessitates a certain level of bootstrapping before moving to code, which fortunately comes very easily with Jekyll. I make use of the [Jekyll Assets](https://github.com/ixti/jekyll-assets) gem for compilation of my frontend assets, providing the familiar [Sprockets](https://github.com/sstephenson/sprockets) pipeline available with Rails.

[Jekyll Haml](https://github.com/samvincent/jekyll-haml) provides me with the minimalistic templating I adore and offers salvation from the ERB style of torture. I also use [Jekyll Content Blocks](https://github.com/rustygeldmacher/jekyll-contentblocks) for Rails style content_for/yielding, generally where I want to render an aside with a page.

Despite nearly all my professional work involving heavy Javascript these days, I took great pleasure in not introducing a single line of Javascript here. There is a certain beauty in the simple application of  styles to markup.

The website is hosted on Amazon S3, for less than $1 per month, and is easily deployed via the [s3 website](https://github.com/laurilehmijoki/s3_website) gem.

## You can find the source code, and possibly some sweary commit messages, on [Github](https://github.com/chrsgrrtt/Abstraktion).
