# Input And Output
To create programs that are user friendly and interactive, you’ll need to know how to output data to a screen and how to get input from a user.

# My Learning Goal
Differentiate between the print and puts commands.
Describe the method used to get input from the user.


# Let start with Output
o output information, such as into your irb or REPL environment or into the command line, we can use the print command. 

use irb in ur terminal
# We can also use the print command:

irb(main):001:0> print "Learning to code is FUN!"
Learning to code is FUN!=> nil

irb(main):002:0> print "1234"
1234=> nil



# We can also use the puts command:
irb(main):001:0> puts "Learning to code is cool!!"
Learning to code is cool!!
=> nil

irb(main):002:0> puts "Hey, I want 2 key lime pies."
Hey, I want 2 key lime pies.
=> nil

irb(main):003:0> x = "My name is ALEX! :)"
=> "My name is ALEX! :)"

irb(main):004:0> puts x
My name is ALEX! :)
=> nil

uts appends a new line to the argument passed in, whereas print keeps things all on one line. A very important thing to notice for both commands is that after printing whatever argument they are passed, puts and print both return nil.



# Input Commands
To accept input from a user, we can use the gets command. When we use gets, program execution will stop and wait for user input. After the user presses Enter, the program will continue its execution.

Again open ur terminal

irb(main):001:0> gets
The progammer from MoringaSchool
=> "The programmer from MoringaSchool\n"

You’ll notice that, unlike puts and print, gets actually returns the user input instead of returning nil. This means that the input can be assigned to a variable for you to then use and manipulate and twist and turn and spit back out.

As you might also remember from the String section of the Basic Data Types lesson, "\n" is an escape character that represents a new line. The gets command always returns a new line at the end of the input. This command often makes use of a “separator” to read streams and multi-line files, but that’s beyond the scope of this beginner lesson. For now, it’s helpful to know that #chomp is a method commonly used to trim separators.


irb(main):001:0> new_string = gets.chomp
This is a sentence.
=> "This is a sentence."

irb(main):002:0> puts new_string
This is a sentence.
=> nil