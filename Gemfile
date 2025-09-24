source "https://rubygems.org"

gem "jekyll", "~> 4.3.0"

# Add missing gems for Ruby 3.4
gem "logger"
gem "csv"
gem "base64"

# Plugin gems for Jekyll
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-seo-tag", "~> 2.8"
  gem "jekyll-sitemap", "~> 1.4"
end

# Windows and JRuby tzinfo-data support
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Lock http_parser.rb on JRuby builds
gem "http_parser.rb", "~> 0.6.3", :platforms => [:jruby]
