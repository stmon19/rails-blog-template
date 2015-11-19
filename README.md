# Getting started

```
mkdir {name}
cd {name}
vim Gemfile
  replace Gemfile like this repogetory
bundle install --path vendor/bundle
bundle exec rails new -B -T -d mysql .
vim config/database.yml
bin/rails g refinery:cms --fresh-installation
bin/rails g rspec:install
bundle exec spring binstub rspec
```
