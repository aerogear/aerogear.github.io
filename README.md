# aerogear.org

## Requirement

Before you can run the side, make sure you have [asciidoc](http://www.methods.co.nz/asciidoc/) installed on your machine!

## Building

1. Install rvm (https://rvm.io/)
1. Run `rvm install ruby 2.1.2`
1. Run `rvm gemset create aerogear`
1. Run `rvm use ruby-2.1.2@aerogear`
1. Run `bundle install --path vendor` to install the dependencies
1. Run `bundle exec jekyll serve --watch`
1. go to <http://127.0.0.1:4000/>
1. profit!

## Publication Info

Pushing to `master` branch, will trigger a Jenkins CI build, which will deploy to <http://staging.aerogear.org>.

Pushing to `production` branch, deploys the site to <http://aerogear.org>.

### Development Steps

. Make changes in aerogear.org repo on a custom branch
. Create a pr against master
. Get the changes reviewed and verified
. Merge to master (which publishes to staging)
. Get the changes verified
. Merge to production branch (which publishes to the site)
