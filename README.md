alecto2
=======

demo app

Last login: Wed Feb  6 13:31:24 on ttys000
rkrao1-mac01:~ Anita$ cd ~/rails_projects
rkrao1-mac01:rails_projects Anita$ rails new demo_app
       exist  
   identical  README.rdoc
   identical  Rakefile
   identical  config.ru
   identical  .gitignore
   identical  Gemfile
       exist  app
   identical  app/assets/images/rails.png
   identical  app/assets/javascripts/application.js
   identical  app/assets/stylesheets/application.css
   identical  app/controllers/application_controller.rb
   identical  app/helpers/application_helper.rb
       exist  app/mailers
       exist  app/models
   identical  app/views/layouts/application.html.erb
   identical  app/mailers/.gitkeep
   identical  app/models/.gitkeep
       exist  config
   identical  config/routes.rb
   identical  config/application.rb
   identical  config/environment.rb
       exist  config/environments
   identical  config/environments/development.rb
   identical  config/environments/production.rb
   identical  config/environments/test.rb
       exist  config/initializers
   identical  config/initializers/backtrace_silencers.rb
   identical  config/initializers/inflections.rb
   identical  config/initializers/mime_types.rb
    conflict  config/initializers/secret_token.rb
Overwrite /Users/Anita/rails_projects/demo_app/config/initializers/secret_token.rb? (enter "h" for help) [Ynaqdh] no
        skip  config/initializers/secret_token.rb
   identical  config/initializers/session_store.rb
   identical  config/initializers/wrap_parameters.rb
       exist  config/locales
   identical  config/locales/en.yml
   identical  config/boot.rb
   identical  config/database.yml
       exist  db
   identical  db/seeds.rb
       exist  doc
   identical  doc/README_FOR_APP
       exist  lib
       exist  lib/tasks
   identical  lib/tasks/.gitkeep
       exist  lib/assets
   identical  lib/assets/.gitkeep
       exist  log
   identical  log/.gitkeep
       exist  public
   identical  public/404.html
   identical  public/422.html
   identical  public/500.html
   identical  public/favicon.ico
   identical  public/index.html
   identical  public/robots.txt
       exist  script
   identical  script/rails
       exist  test/fixtures
   identical  test/fixtures/.gitkeep
       exist  test/functional
   identical  test/functional/.gitkeep
       exist  test/integration
   identical  test/integration/.gitkeep
       exist  test/unit
   identical  test/unit/.gitkeep
   identical  test/performance/browsing_test.rb
   identical  test/test_helper.rb
       exist  tmp/cache
       exist  tmp/cache/assets
       exist  vendor/assets/javascripts
   identical  vendor/assets/javascripts/.gitkeep
       exist  vendor/assets/stylesheets
   identical  vendor/assets/stylesheets/.gitkeep
       exist  vendor/plugins
   identical  vendor/plugins/.gitkeep
         run  bundle install
Using rake (10.0.3) 
Using i18n (0.6.1) 
Using multi_json (1.5.0) 
Using activesupport (3.2.8) 
Using builder (3.0.4) 
Using activemodel (3.2.8) 
Using erubis (2.7.0) 
Using journey (1.0.4) 
Using rack (1.4.4) 
Using rack-cache (1.2) 
Using rack-test (0.6.2) 
Using hike (1.2.1) 
Using tilt (1.3.3) 
Using sprockets (2.1.3) 
Using actionpack (3.2.8) 
Using mime-types (1.20.1) 
Using polyglot (0.3.3) 
Using treetop (1.4.12) 
Using mail (2.4.4) 
Using actionmailer (3.2.8) 
Using arel (3.0.2) 
Using tzinfo (0.3.35) 
Using activerecord (3.2.8) 
Using activeresource (3.2.8) 
Using coffee-script-source (1.4.0) 
Using execjs (1.4.0) 
Using coffee-script (2.2.0) 
Using rack-ssl (1.3.3) 
Using json (1.7.6) 
Using rdoc (3.12.1) 
Using thor (0.17.0) 
Using railties (3.2.8) 
Using coffee-rails (3.2.2) 
Using jquery-rails (2.2.0) 
Using bundler (1.1.5) 
Using rails (3.2.8) 
Using sass (3.2.5) 
Using sass-rails (3.2.6) 
Using sqlite3 (1.3.7) 
Using uglifier (1.3.0) 
Your bundle is complete! Use `bundle show [gemname]` to see where a bundled gem is installed.
rkrao1-mac01:rails_projects Anita$ git init
Initialized empty Git repository in /Users/Anita/rails_projects/.git/
rkrao1-mac01:rails_projects Anita$ git add .
rkrao1-mac01:rails_projects Anita$ git remote add origin git@github.com:<anita5r>/demo_app.git
-bash: anita5r: No such file or directory
rkrao1-mac01:rails_projects Anita$ git remote add origin git@github.com:<anita5r>/alecto.git
-bash: anita5r: No such file or directory
rkrao1-mac01:rails_projects Anita$ bundle exec rake db:migrate
Could not locate Gemfile
rkrao1-mac01:rails_projects Anita$ rails generate scaffold User name:string email:string
Usage:
  rails new APP_PATH [options]

Options:
  -r, [--ruby=PATH]              # Path to the Ruby binary of your choice
                                 # Default: /usr/local/rvm/rubies/ruby-1.9.3-p194/bin/ruby
  -b, [--builder=BUILDER]        # Path to a application builder (can be a filesystem path or URL)
  -m, [--template=TEMPLATE]      # Path to an application template (can be a filesystem path or URL)
      [--skip-gemfile]           # Don't create a Gemfile
      [--skip-bundle]            # Don't run bundle install
  -G, [--skip-git]               # Skip Git ignores and keeps
  -O, [--skip-active-record]     # Skip Active Record files
  -S, [--skip-sprockets]         # Skip Sprockets files
  -d, [--database=DATABASE]      # Preconfigure for selected database (options: mysql/oracle/postgresql/sqlite3/frontbase/ibm_db/sqlserver/jdbcmysql/jdbcsqlite3/jdbcpostgresql/jdbc)
                                 # Default: sqlite3
  -j, [--javascript=JAVASCRIPT]  # Preconfigure for selected JavaScript library
                                 # Default: jquery
  -J, [--skip-javascript]        # Skip JavaScript files
      [--dev]                    # Setup the application with Gemfile pointing to your Rails checkout
      [--edge]                   # Setup the application with Gemfile pointing to Rails repository
  -T, [--skip-test-unit]         # Skip Test::Unit files
      [--old-style-hash]         # Force using old style hash (:foo => 'bar') on Ruby >= 1.9

Runtime options:
  -f, [--force]    # Overwrite files that already exist
  -p, [--pretend]  # Run but do not make any changes
  -q, [--quiet]    # Suppress status output
  -s, [--skip]     # Skip files that already exist

Rails options:
  -h, [--help]     # Show this help message and quit
  -v, [--version]  # Show Rails version number and quit

Description:
    The 'rails new' command creates a new Rails application with a default
    directory structure and configuration at the path you specify.

    You can specify extra command-line arguments to be used every time
    'rails new' runs in the .railsrc configuration file in your home directory.

    Note that the arguments specified in the .railsrc file don't affect the
    defaults values shown above in this help message.

Example:
    rails new ~/Code/Ruby/weblog

    This generates a skeletal Rails installation in ~/Code/Ruby/weblog.
    See the README in the newly created application to get going.
rkrao1-mac01:rails_projects Anita$ 
