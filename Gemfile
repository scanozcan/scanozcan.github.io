source "https://rubygems.org"

# Updated for Ruby 4.0.1
gem "jekyll", "~> 4.4.1"
gem "minima", "~> 2.5"
gem "webrick", "~> 1.7"

# Remove ffi version restriction for newer Ruby
gem "ffi"

# Required for GFM markdown
gem "kramdown-parser-gfm"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"
  gem "jekyll-seo-tag", "~> 2.8"
end

# Windows and JRuby does not include zoneinfo files
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]
