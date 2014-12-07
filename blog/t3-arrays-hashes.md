Should I use an Array or Hash

Lets start out with a quick overview of what exactly an Arrays' and Hashs' are. First Array, an array is an easy way of storing data. Once data is in an array it is also fairly easy to access that data, if you know where to look. Below is quick example of creating an Array and getting the information out of it.

```Ruby
#This is just one way of creating an array note there are multiple.
some_stuff = ["Spider man", 2, true]

puts some_stuff[0]
#Prints "Spider man" important to note that arrays counting starts at 0

puts some_stuff[1]
#Prints 2

puts some_stuff[2]
#Prints true
```
now I'll get into when to use an array in a second but first let me show show you how to create and use a Hash, for simplisty I will only show you one way off creating a Hash but there are mutliple.

```Ruby

menu = Hash.new

menu["chicken"] = "yum"
menu["soup"] = 13
menu["dog"] = false

puts menu["chicken"]
#Puts 52

puts menu["soup"]
#Puts 13

puts menu["dog"]
#Puts 83
```

As you can see Hash are quite different from Arrays. They both hold data sets, but with Hash you refrence the data with a key word rather than a number. It's sort of like you are creating a list of vairbles. As of Ruby 1.9 there is a order to a Hash set however you don't really refrence things from that order, as opposed to an Array which has a clearly defined order.

Hash's are must faster for doing a random search in, for example if you had a bunch of kids names and their test scores, it is much easier and more effcient to do:

```Ruby

grade = Hash.new

grade["Peter"] = 100
grade["Sam"] = 78

puts grade["Peter"]
```

Then it would be to do the same thing with an array:

```Ruby
grade = [["Peter", 100],["Sam",78]]

puts grade[0][1]

```

For the second example you would have to know the place of every student in order to get their grade, but with a Hash you can just type their name. However, to be fair to Arrays Hashs' are not always the best choice. Anything that needs a numerical order you should you use a Array for and just about everything else use a Hash.