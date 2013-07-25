# Takeaways from LoneStarRuby

## Random
* interesting podcast: Realtalk 
* perftools.rb
* Async Ruby Jobs: Resque (like delayed job but with Redis)


## Application Performance
* perftools.rb
* DTrace

## Good low level books
* Ruby Under a Microscope
* Working With TCP Sockets
* Working With Unix Processes

## getting into trouble
* nmap
* burp as a proxy
* BeFF
* metaprogramming ruby: <https://speakerdeck.com/anthonylewis/advanced-ruby>

## random ruby fact
	extend SomeModule # import module methods as class methods
	include SomeModule # import module methods as class methods
	
	# there's a callback when you include a module
	module AnotherModule
	  def self.included(base)
	    base # the class including this module
	  end
	end

## code quality ideas
* **write down agreed upon style guide**
	* go into a room dont leave until decided upon
	* ruthless adherence
	* out-of-band litigation process (ie review in 1 month)
* **lunch and learn**
	* like are brown bagging
	* instead maybe lunch plus a confreak video we vote on
	* every other wednesday
* **team refactoring**
	* one hour
	* everyone on the team
	* output not important
	* **the conversation is the value**
	* see and discuss different styles/patterns/etc
	* rotate lead
	* every week
* **whiteboarding**
	* overall design/architecture
* **code review**
	* github
	* non-blocking
	* opt-in (let dev writing code have final say)
	* review criteria: **comrehension most important**
* **time block a new process**
	* trying out a new process
	* have a set amount of time to try
	* then at the end evalua and continue, discontinue, or modify
* **boy scout rule**
	* fix something while working in it
	* over time overall code quality goes up