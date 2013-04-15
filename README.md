# SeemsRateable

Star rating gem for Rails application using jQuery plugin jRating

## Demo

<a href="http://rateable.herokuapp.com/">Demo</a> application, requires to sign up before rating 

## Instructions

### Installation

Add this line to your application's Gemfile:

    gem 'seems_rateable'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install seems_rateable

### Generation

    $ rails g seems_rateable User
    
Generator takes one argument which is name of an existing user model e.g User, Client, Player ... <br>
The generator creates necessary model, controller and asset files. It also creates route and migration files that are already migrated

### Prepare
    
Include Javascript files adding these lines to application.js

     //= require rateable/jRating.jquery
     //= require rateable/rateable.jquery
     
Include CSS file adding <code><%= seems_rateable_style %></code> to your layaut head tag

To prepare model be rateable add <code>seems_rateable</code> to your model file. You can also pass a hash of options to 
customize the functionality

<ul>
<li><code>:dimensions</code> Array of dimensions e.g. <code>:dimensions => [:quality, :price, :performance]</code></li>
<li><code>:allow_update</code> Allowing user to re-rate his own ratings, default set to false e.g <code>:allow_update=> true</code>
<ul>

    class 

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
