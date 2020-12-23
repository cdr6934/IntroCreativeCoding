# Quick Start Creative Coding 


The following article will provide an introduction on how to get started with creative coding. 

But first, I have a secret to tell you. 

Code, is not just for smart people. It isn't a lofty ledge that only the best reach.  You can understand it too! Now, there is a learning curve and it won't come easily if you aren't just playing around with the code. And more importantly you have to remember that code is a type of thinking. You learn to think like a computer. 

A *program* is a packaged set of instructions that run on your computer. The code that you are going to be writing is the DNA of the program. So you get to play the creator and write code to make the program do whatever you wish. 

Now computers that run the programs talk in 1010100. Which if we had to write our code this way, it would take much too long. So we get to write a program in a human readable language. This is when you have heard people call programming languages like BASIC, javascript or C++. These languages are written in such a way that it makes it easy for us average people to read and write them. They have a different sentence structure than the English language, but we will slowly walk through those as we get around to them. 


Once we have written it in a language, the language gets compiled, or translated into 101010 so your computer knows what to do with it. And then we get to see the output of the program that we have written. Its that easy. 

Lets get started by downloading the software we need. 

## Installing Processing 
* Go to www.processing.org
* Download to your computer 
* Install 
* Open the text editor or IDE (Integrated Development Environment) - or think of it as the Walmart of programming. You find everything you need to write your program. 

So once you have everything installed you will open up your Processing program. 

![](/media/ide.png)

There are a few elements of the program structure.

A `variable` is the name you can give a piece of information either a number or text that can be changed at any point during the lifecycle of the program. For example, if you wanted to keep a tally of how many times something runs. 

The `type` is an important concept and can be a little scary at first. 
 
A `function` is a block of code, or a set of instructions that is reusable. Think of it as a recipe of code. It is an easy way to group sets of instructions together so that it is organized and reusable. 


It is for anyone willing to give it a try. There are many tools 


``` java
void setup() 
{

}

void draw() 
{
	print(1+1); 
}
```
The output looks like this...

![Terminal Output](/media/creativecoding_1.gif)

> Why is this? Take a second and try to figure out why this might be.  

You can see in the terminal window, the two continues to show and you can see that it signifies that the draw() function has run the count of 2s times. 


This is an important concept to remember as you are working in any language. But in Processing; these special functions have different purposes.  `void setup()` is run once at the beginning of the program's lifetime. 

And then **never** again until the program is restarted. 

However, the `draw()` function will continue to run again and again until it is told to stop. 


``` java 
void setup() 
{
	size(100, 100); #The size of the window 
	background(255); # color of the background
}

void draw() 
{
	stroke(0); 
	line(width/2, height/2, (width/2)*30, height/2); 
}
```
Yay! We have a line! That is great and is a basic element of doing all sorts of amazing things. 

Now we can do something even more interesting and learning that will come soon but for now, we are going to add a random function into your program to give you something exciting. 

``` java

void setup() 
{
  size(1000,1000);
  background(255);
}

void draw() 
{
  line(random(width), random(height),random(width), random(height)); 
}
```

Congratulations! You have written your first program! 

![50 Random Lines](/media/random_lines_2.gif)


### Gotchas
> Remember to always end every line that is not a function or a collection of functions called a **class**.