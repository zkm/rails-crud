# Rails-CRUD

## Prerequisites

The setups steps expect following tools installed on the system.

- Github
- Ruby [3.1.2]
- Rails [7.0.4]

### 1. Clone the repository

```bash
git clone git@github.com:zkm/rails-crud.git
```

### 2. Confirm you have Ruby and Rails installed 
```bash
ruby --version && rails --version
```

### 3. Install bundler
```bash
gem install bundler 
```

### 4. Run the bundler
```bash
bundle install  
```

### 5. Create and setup the database

Run the following command to create and setup the database.

```ruby
rake db:migrate
```

### 6. Add some data so we can run tests

Run the following command to seed database.

```ruby
rake db:seed
```

### 7. Start the Rails server

You can start the rails server using the command given below.

```ruby
bundle exec rails s
```

If port 3000 is already in use, you can either:
- Stop the existing server: `lsof -ti:3000 | xargs kill -9`
- Use a different port: `bundle exec rails s -p 3001`

### 8. View routes

Run the following command or go to http://localhost:3000/rails/info/routes to see all routes your application is configured to. 

```ruby
rails routes
```

And now you can visit the site with the URL http://localhost:3000/dogs
