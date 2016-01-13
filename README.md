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

### Additional way of model
```
# sample
bin/rails g refinery:engine work title:string image:image description:text material:string size:string completed_at:datetime

# Add author to vendor/extension gemspec
vim vendor/extension/works/refinery-cms-works.gemspec
  s.author            = 'your name'

bundle install --path vendor/bundle
bin/rails generate refinery:works
bin/rake db:migrate
bin/rake db:seed
```
