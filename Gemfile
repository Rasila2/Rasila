source "https://rubygems.org"

# This will help ensure the proper Jekyll version is running.
gem "jekyll", "~> 4.3.0"

# If you want to use GitHub Pages, remove the "gem "jekyll"" above and
# uncomment the line below. To upgrade, run `bundle update`.
# gem "github-pages", group: :jekyll_plugins

group :jekyll_plugins do
  gem 'jekyll-paginate'
  gem 'jekyll-sitemap'
  gem 'jekyll-feed'
  gem 'jekyll-seo-tag'
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
# Temporarily commented out due to compatibility issues
# gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Required for Ruby 3.0+
gem "webrick", "~> 1.8"

# Required gems for Ruby 3.3+
gem "csv", "~> 3.2"
gem "base64", "~> 0.2.0"
gem "bigdecimal", "~> 3.1"

