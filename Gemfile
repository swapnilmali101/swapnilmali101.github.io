source "https://rubygems.org"

# Use core Jekyll version
gem "jekyll", "~> 4.3"

# Your theme
gem "jekyll-theme-chirpy", "~> 7.4"

platforms :windows, :jruby do
# If you are running this locally on Windows/Linux, you might need these:
group :jekyll_plugins do
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
  gem "webrick" # Required for Ruby 3.0+ local server
end

gem "wdm", "~> 0.2.0", :platforms => [:windows]

# test script
group :test do
  gem "html-proofer"
end
