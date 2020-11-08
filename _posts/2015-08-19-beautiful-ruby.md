---
layout: post
title:  "Beautiful Ruby"
date:   2014-08-19 13:06:02
categories: ruby update
---

 Ruby is a programming language that is a general purpose language and suitable for a multitude of purposes. Created with a programmers happiness in mind it has become well known for the simplicity of source generated while still allowing impressive and powerful features.

## Data structures

```ruby
str = "this is a string"
array = ["first", "second", "third"]
hash = { "key" => "value", "next_one" => "its value" }
```

Here is an example of a couple declarations within Ruby. The key take away is the fact that it is dynamically typed. Arrays and hashes are the more powerful data types that are used when programming with Ruby.

## Defining methods

```ruby
def method_declaration(string_arg)
  string_arg.upcase
end
```

Although it looks as though it won’t return a value this method will return the upcased version of the argument string that is passed in. The last evaluated expression is the return value for methods. Makes for less code and less cluttered as well. Often times you will find yourself composing methods in domain specific meaningful ways.

## Expression calls

```ruby
str = "the,quick,brown,fox,jumps,over,the,lazy,dog"
str.split(,).join(' ').gsub("the", "a").upcase
```

Speaking of readable code. This example highlights that fact that you created quite closely to a human readable line that explains (self-documents) what it is doing. That being said I wouldn’t recommend going over board with chaining messages like this together. Makes debugging a big headache as you often need to resort to breaking the method calls into separate lines to determine problem.

## Conditionals

```ruby
is_true = true
if is_true
  puts "is_true is true"
end
```

Nothing special here I feel. Not especially flashy, but really that is part of the beauty of Ruby. Here we have a stripped down if statement compared to many other languages that exist. For example the if condition syntax for Javascript is busy relative to this.

## Loops

```ruby
collection = Array (1..10)
collection.each do |item|
  puts item
end
```

Little more flashiness going on here. First we create an Array populated with the numbers 1 through 10 and then pass the message .each in order to invoke the loop. Within the loop we call puts with the argument of item (puts is a type of Ruby print statement) to display all the items in the Array collection. Kind of a mouthful to type that up in plain English compared to Ruby…

Hopefully this quick little intro introduced some of the fundamentals of programming that can be done with Ruby. Sometime I will need to touch base on the Object Oriented principles of Ruby.
