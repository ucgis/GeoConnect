source "https://rubygems.org"

# GitHub Pages gem (includes Jekyll and compatible versions)
gem "github-pages", group: :jekyll_plugins

# Plugins
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-seo-tag"
end

# Windows and JRuby does not include zoneinfo files
platforms :windows do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance booster for Windows
gem "wdm", "~> 0.1", platforms: [:mingw, :x64_mingw, :mswin]

# JRuby compatibility
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]
