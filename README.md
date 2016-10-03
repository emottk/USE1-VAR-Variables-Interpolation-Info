#>> VARIABLES & INTERPOLATION
###*Just like math, but cooler.*


You're creating a new chatbot, and you want it to greet users the same way every single time you run it:

`"Hello! My name is BotoTron, I am here to talk at you."`

Easy enough. But now we want to send that off to our 50 million users over and over again. That's a lot of text to be reproducing every time someone tries to talk to our bot.		

Ruby has a solution to this problem - in fact, most languages do. They're called **variables**, and they're super useful.		
Instead of rewriting that string everytime we need to use it, we can instead store it inside of a variable, like so:

	greeting = "Hello! My name is BotoTron, I am here to talk at you."
	
A variable is a placeholder for a piece of data (string, integer, boolean, etc). Now, if we call `greeting`, our string will print to the screen.

	print greeting
	  >>"Hello! My name is BotoTron, I am here to talk at you."
	 
We can use variables to print something multiple times:

	hey = "HEY HEY HI "
	print hey*5
	   >> "HEY HEY HI HEY HEY HI HEY HEY HI HEY HEY HI HEY HEY HI "

We can also use variables within our strings. This is called **string interpolation**.

	name = Jenny
	"Hi #{name}, how are you?"
		>>"Hi Jenny, how are you?"

Here we use the `#{ }` interpolation syntax to inject our variable into our string. When Ruby runs the program, it will find the variable called `name` and print it inside the string. This is great, now we can personalize all of our strings!

Variables can be assigned to any data type, not just strings. We can also interpolate integers inside strings: 

	year = 2016
	"It is the year #{year}"
		>>"It is the year 2016"

Order matters with variable assignment.
	
	name = Bobby
	age = 14
	name = Jimmy
	
	introducction = "Hi my name is #{name}, and I am #{age} years old.

What do you think Ruby will print for `introduction`?

	print introduction
		>> "Hi my name is Jimmy, and I am 14 years old."

That's right, whatever was assigned last is what Ruby uses as the variable value. 

Test your knowledge of variables with a fun [Ruby variables Kahoot!](https://play.kahoot.it/#/k/654fb064-ff29-46b8-8f20-568c65d54d2d)
	



