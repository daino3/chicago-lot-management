## Responsive Sinatra Form w/ Stripe Integration

Couple niceties:
+ Rails-like folder structure
+ [Foundation](http://foundation.zurb.com/docs/) responsive framework 
+ Postgres database config
+ Underscore.js 
+ Slim templating engine
+ Stripe integration w/ quantity-based subscription
+ Rspec testing framework
+ Bare-bones admin route for viewing subscriptions 

### Setup
Clone the Repo
```
git clone git@github.com:daino3/chicago-lot-management.git
```
Change into the directory and run:
```
bundle install
```
### Running Server Locally
Default set to 3000 in config.ru
```
bundle exec rackup
```
### Running Specs
```
bundle exec rspec spec
```

### Heroku
1. Install the [Heroku Toolbelt](https://toolbelt.heroku.com/)
2. Get Heroku credentials from Heroku account owner or be made a contributor to the project
3. Connecting to Existing Heroku Application

```
git remote add heroku <GIT@HEROKU.COM:HEROKU-APP-NAME.GIT>
```

### Subscription Routes
Note: Don't change the plan names / ids in the Stripe dashboard or these will fail 
* /subscribe-observation
* /subscribe-basic
* /subscribe-premium
* /subscriptions/create

### Admin Routes
* /admin
