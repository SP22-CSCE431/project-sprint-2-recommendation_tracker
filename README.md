# README

## Introduction ##

This application was made for Dr. Lightfoot, a Computer Science professor at Texas A&M University. The purpose of this application is to store information about all of Lightfoot's students, so he can create more personalized and genuine recommendation letters.

## Requirements ##

This code has been run and tested on:

* Ruby - 3.0.2p107
* Rails - 6.1.4.1
* Ruby Gems - Listed in `Gemfile`
* PostgreSQL - 13.3 
* Nodejs - v16.9.1
* Yarn - 1.22.11


## External Deps  ##

* Docker - Download latest version at https://www.docker.com/products/docker-desktop
* Heroku CLI - Download latest version at https://devcenter.heroku.com/articles/heroku-cli
* Git - Downloat latest version at https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

## Installation ##

Download this code repository by using git:

 `git clone https://github.com/your_github_here.git`


## Tests ##

An RSpec test suite is available and can be ran using:

  `rspec spec/`

## Execute Code ##

Run the following code in Powershell if using windows or the terminal using Linux/Mac

  `cd your_github_here`

  `docker run --rm -it --volume "$(pwd):/rails_app" -e DATABASE_USER=test_app -e DATABASE_PASSWORD=test_password -p 3000:3000 dmartinez05/ruby_rails_postgresql:latest`

  `cd rails_app`

Install the app

  `bundle install && rails webpacker:install && rails db:create && db:migrate`

Run the app
  `rails server --binding:0.0.0.0`

The application can be seen using a browser and navigating to http://localhost:3000/

## Environmental Variables/Files ##

If you want to duplicate this application locally, you will need to set up Google OAuth for user login. Instructions can be found here: https://medium.com/@adamlangsner/google-oauth-rails-5-using-devise-and-omniauth-1b7fa5f72c8e. When setting up your own Google OAuth make sure to save the following environmental variables:

`GOOGLE_OAUTH_CLIENT_ID`
`GOOGLE_OAUTH_CLIENT_SECRET`

and save them into your development.rb file


## Deployment ##

** Add instructions about how to deploy to Heroku

we created a video to walkthrough how to deploy the app on Heroku. You should have a github account with this code and an Heroku account linked to your email. If you need any help please email yk7335@tamu.edu for any questions. The video walks through creating pipeline and adding apps to test, staging, and production areas. 

The linke is: https://drive.google.com/file/d/1skh4dptZLSv8B1wBKtFzcAInd_9ww17t/view?usp=sharing


## CI/CD ##

We use github actions to run the gems rubocop, brakeman, and rspec.

## Support ##

Admins looking for support should first look at the application help page.
Users looking for help seek out assistance from the customer.

