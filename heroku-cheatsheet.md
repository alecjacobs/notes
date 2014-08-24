Heroku Cheatsheet
=

A personal cheatsheet for getting an app up and running on Heroku

prerequisites
-
- ruby
- rails
- postgres

steps
-

1. create app on heroku
2. clone the repo locally
3. in the cloned directory

	<pre>rails new . </pre>

4. do a blank app commit
5. add gems needed for heroku 

	<pre>
	gem 'rails_12factor', group: :production
	gem 'pg'</pre>

6. bundle & commit
7. setup local dev db config

	<pre>
	development:
	  adapter: postgresql
	  host: localhost
	  username: [LOCAL-USERNAME]
	  database: app-dev</pre>

8. create a controller

	<pre>rails g controller Welcome</pre>

9. add a basic index action

	<pre>
	def index
	  render plain: "howdy!"
	end</pre>

10. setup the route

	<pre>root 'welcome#index'</pre>
	
11. push to heroku
	<pre>git push heroku master</pre>

done!
-


Useful links:

- https://devcenter.heroku.com/articles/rails4#postgres



