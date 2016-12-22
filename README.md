# Rails Commands Quiz

Fork, clone, and write your answers directly in this file. Then submit a pull request.

### Question 1

I want to start a new Rails project/app called `BunnyApp`. What command should I type in the terminal?
"rails new BunnyApp" , if you wanted to use postgresql you would specify with a -d and the name postgresql

### Question 2

I want to create a new model called `Bunny`, with the following attributes: name (string), color (string), and age (integer). What command(s) should I type in the terminal and/or Sublime? (In your answer, create both a migration and the model file.)

rails g model Bunny name:string color:string age:integer

### Question 3

What does the command in Question 2 do, exactly? What files are created, where are they located, and what does the database look like at this time? Explain.

it generated a model named bunny in your models which inherets from appicationrecord ,which inheret form activerecord::base
also generates a migration prepopulated with the the data that will be both the columns and the expected datatype. and finally two test files. The database remains unchanged until you run a migration.


### Question 4

I want to create a database and make it reflect the new model I created in Question 2. What command(s) should I type in the terminal?

rake db:migration

### Question 5

I want to look at the actual database that has been created. What command should I type in the terminal?


rails c
to go to the database in console.

### Question 6

I want to see a list of all the URLs available in my app, along with the HTTP requests and controllers associated with them. What command should I type in the terminal?

rake routes or rails routes

### Question 7

What line should I add to `config/routes.rb` to create a complete set of RESTful routes for a "bunnies" resource?

resources :bunnies

### Question 8

According to standard Rails conventions, what directory and filename would the BunniesController be located in, starting from the root of the project?

app > controllers > bunnies_Controller.rb

### Question 9

According to standard Rails conventions, what directory and filename would the "show" view for bunnies be located in, starting from the root of the project?

app > views > bunnies > show.html.erb

### Question 10

I have worked on my app and finally want to see it in action. What command should I type in the terminal, and where should I navigate to in my browser?


rails s  ,  by default the port is set to 3000
http://localhost/3000
