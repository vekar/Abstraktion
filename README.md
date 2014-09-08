# Abstraktion

My Jekyll powered blog and portfolio. I chose to open source this to provide a starting point for anyone looking to rapidly develop websites with [Jekyll](http://jekyllrb.com/).

### Getting started

The website is powered by Jekyll and uses a number of Ruby gems to aid frontend development. Getting started is easy though, simply `git clone` the repository and from it's root install gem dependencies with `bundle install --path vendor/bundle`.

You should now have dependencies, like [Jekyll Assets](https://github.com/ixti/jekyll-assets) installed, so go ahead and start jekyll with `bundle exec jekyll serve --watch`. You should now be able to [view the website](http://0.0.0.0:4000).

### Development

All content and assets live in the [source directory](source). The Jekyll assets Gem provides sprockets style compiling and serving of assets. I've used [SASS](http://sass-lang.com/) and [compass](http://compass-style.org/) for elegant stylesheets. Content, where possible is written in markdown, for more complex views, I've used [HAML](http://haml.info/).

### Deployment

I serve the website directly from S3. Deployment comes courtesy of the [S3 website](https://github.com/laurilehmijoki/s3_website) Gem. In order to deploy, an `s3_website.yml` will need to be added to the root of the project, similar to this:

`s3_id: ABC
s3_secret: XYZ
s3_bucket: 123

s3_endpoint: eu-west-1

gzip:
  - .html
  - .css
  - .md

gzip_zopfli: true

s3_reduced_redundancy: true`

The website can then be built and deployed with: `bundle exec jekyll build && bundle exec s3_website push`.

