source "https://rubygems.org"
ruby RUBY_VERSION

require "json"
require "open-uri"
versions = JSON.parse(open('https://pages.github.com/versions.json').read)

gem "github-pages", versions["github-pages"]
gem "jekyll-assets"
gem "jekyll-feed", "0.8.0"
gem "jekyll-haml"
gem "coffee-script"
gem "font-awesome-sass"
gem "bourbon", "5.0.0.beta.7"
gem "neat"
gem "sass"
gem "uglifier"
gem "octopress-autoprefixer"
gem "turbolinks"
