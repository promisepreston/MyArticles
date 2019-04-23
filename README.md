# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version - 2.5.1

* Rails version - 5.2.2

* Database Type - RDMS (Sqlite 3)

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...



# Lessons Learnt

1. Use the Module scope in the controllers when you add controllers to folders in the controllers folder
E.g module Api
      module V1
        class ArticlesController < ApplicationController
2. Use the Namespace scope in the routes when you add controllers to folders in the controllers folder
E.g. namespace 'api' do
        namespace 'v1' do
          resources :articles
        end
     end
3. Use the Faker Gem for generating fake data for the models
4. Use the Rails Console to check your data anytime you add you add new data
E.g rails console
    Articles.all
5. Use rake routes to see your routes anytime you add new routes.
E.g rails routes
6. Use Postman to test the APIs to ensure that they are functional.
7. When testing in Postman, use the default URL for all CRUD operations if you used the resources for your route
E.g. Use http://localhost:3000/api/v1/articles for all CRUD operations and not http://localhost:3000/api/v1/articles/create for Creating Articles or http://localhost:3000/api/v1/articles/update for Updating 

#Source
https://medium.com/@hunter.j.nate/well-the-jerk-store-called-and-they-said-you-didnt-know-how-to-build-an-api-120eda19c836

