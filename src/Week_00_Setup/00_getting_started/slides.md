![GeneralAssemb.ly](/img/icons/FEWD_Logo.png)

# Welcome Intro to Ruby on Rails!

---

## Hi! I'm...

* Corey Speisman
* I'm a fullstack developer at [Capterra](http://capterra.com).
* You can email me anytime: [Cspeisman@gmail.com](mailto:Cspeisman@gmail.com).
* I'm [@cdspeis](http://twitter.com/cdspeis) just about everywhere.

---

## Agenda

*	What is programming?
* Intro to ruby
* Intro to object-oriented programming
* Intro to rails

---
### What is programming?

When you teach someone how to make a sandwich, your job is made much easier because they already know what a sandwich is.

--

If you were to tell your computer to make a sandwich you would have to give very specific directions.

* open cabinet 
* see if there is bread
* if there is no bread go to the store and buy bread
* open bread packaging and take out 2 slices

-- 
Programming is telling your computer how to do something.  Large tasks must be broken up into smaller tasks, which must be broken up into even smaller tasks, down until you get to the most basic tasks that you don't have to descibe - and that your computer already knows how to do.

---
## Programming Languages

In order to tell your computer how to do something, you must use a programming language.

--
A programing language is similar to a human langauge in that it's made up of basic elements (such as nouns and verbs) and ways to combine those elements to create meaning.


---
## What is Ruby?

Ruby is a dynamic object oriented pogramming language that is simple, easy to learn, and elegant.

-- 
Perhaps the best reason for using Ruby is that it tends to be short. For example, here's a small program in Java:

	public class HelloWorld {
		public static void main(String []args){
			System.out.println("Hello World");
		}
	}

--
And here's the exact same program in Ruby:

	puts 'Hello World'

---
## Getting started with ruby

We are going to be using [nitrous.io](https://www.nitrous.io/)

please take a few minutes to set up a free account

--

## Let's creat our first program!

--

	puts "what is your name?"
	name = gets.chop
	puts "Hi #{name}, how are you??"

---

## Intro to Ruby

* variables/assignment
* arrays/concatinating and iterations

--
![GeneralAssemb.ly](../img/icons/exercise_icon_md.png)
## Dictionary Sort

Instructions: 
 Prompts user to enter a word
- Tells user to enter another word or hit the return key
- Repeats that process until the user hits the return key
- Returns all the words entered in alphabetical order

---

## Intro to Object Oriented

*  Objects are basic building blocks of Ruby
*  Literally everything is an object in Ruby
*  You can think of Objects as any noun (users, computers , animals, cars, pets, houses, etc..etc)

--
There are two steps to creating an object in ruby

The first is to define a class
--
## Class

Classes are basically your blueprint or a template for your object
		
		class Person
			def initialize(name)
				puts "A user is being created"
			end
		end

A class can be used to create many objects

--

The second step is to instantiate the object (aka create your object from the class)

	person1 = Person.new('Corey')
	person2 = Person.new('Pat')

--

## Anatomy of a class

	class ClassName
	end

class definition starts with the keyword __class__ followed by the __class name__
and is delimited with __end__

--

## Initialize method

	class Box
		def initialize(w,h)
			@width = w
			@height = h
		end
	end

The initialize method is considered our constructor.  It is used when you want to initialize class variables at the same time as creating your class

--

## instance variables
	@width = w
	@height = h

instance variables are class attributes and become properties of the object when an object is instanciated.  They can also be passed between all of the class methods

--

#accessor methods

	# define a class
	class Box
	
		# constructor method
		def initialize(w,h)
			@width, @height = w, h
		end
	
		# accessor methods
		def printWidth
			@width
		end
	
		def printHeight
			@height
		end
	end

	# create an object
	box = Box.new(10, 20)

	# use accessor methods
	x = box.printWidth()
	y = box.printHeight()

accessor methods allow us to access our instance variables from outside of the class

--

![GeneralAssemb.ly](../img/icons/code_along.png)

Let's create a student class where we can store a student's name, a student's id, a student's test scores, and retrieve their gpa

---

## Intro to Rails

--

## Question 1 - What is Ruby on rails?

* Open Source Framework
* Built with and uses the ruby programming language
* Uses MVC framework (model, view. controller)

--
![GeneralAssemb.ly](../img/icons/exercise_icon_md.png)

Let's just jump into and build something cool!
