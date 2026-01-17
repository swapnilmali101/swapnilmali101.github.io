source "https://rubygems.org"

# Use core Jekyll version
gem "jekyll", "~> 4.3"

# Your theme
gem "jekyll-theme-chirpy", "~> 7.4"

# If you are running this locally on Windows/Linux, you might need these:
platforms :windows, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.2.0", :platforms => [:windows]

# test script
group :test do
  gem "html-proofer"
end
