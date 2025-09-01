source "https://rubygems.org"

gem "jekyll", "~> 4.3.0"
gem "csv"
gem "base64"
gem "jekyll-feed", "~> 0.15"
gem "jekyll-seo-tag", "~> 2.8"
gem "jekyll-sitemap", "~> 1.4"

# GitHub Pages plugins
group :jekyll_plugins do
  gem "jekyll-github-metadata"
  gem "jekyll-relative-links"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", platforms: [:mingw, :x64_mingw, :mswin]