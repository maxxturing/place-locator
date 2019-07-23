# README

rails generate scaffold location name:string address:string latitude:float longitude:float
rake db:migrate

to run `rails server`
http://localhost:3000/locations
http://localhost:3000/

Uses geocoder gem (gem install geocoder)
https://github.com/alexreisner/geocoder

Uses kaminari gem (pagination)
https://github.com/kaminari/kaminari

Migrate db for heroku:
1. Install Heroku CLI
2. Install pg gem

group :development,:test do
   gem 'sqlite3'    #gem to use in development environment
end

group :production do
  gem 'pg'         #gem to use in production environment
end

3. Edit config\database.yml

4. heroku run rake db:migrate -a place-locator
