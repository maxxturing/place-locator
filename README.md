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
