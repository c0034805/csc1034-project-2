# Project 2 Report

This is a short report that focuses on how I identified errors in the code
of Project 2. Before I start, I should mention that I had first detected the
errors that I did and then started again from scratch before I started pushing
it back to NUCODE (this is the reason why the Switch().run_game() error is not
the one that is fixed first for example).

Once I cloned the project, I ran the code for the first time to see what I was
dealing with. After fixing a couple of issues that I found from the error
messages of the program crashing, I started looking through the code and went
through how the code goes about running the card game, from the generation of
the deck to the winner of the game, to gain a better understanding of it. This
is  how I found minor logical errors, such as the same person always being 
displayed as victor and other such issues.

When I was sure there were not any more of these kinds of logical errors, I 
went back to running the program until it broke and shuffled through the code
each time to fix whatever was causing it. The program breaking after playing
the Joker card being played issue I discovered this way (among others).

I eventually reached the point where I could play a game from beginning to end
without the program breaking on me. At this point, I consulted the README file
for the rules and began adding the missing rules to the game, such as the Queen
card not forcing the next player to draw four cards, as well as the Queen and 
Ace cards not being discardable whatever the top card. Reading through the 
documentation and comments I also found a few typos, which I corrected.

When the game was practically ready I started looking through the test suite. 
This was my greatest mistake while working on this project. I could have very
likely found the errors I detected previously much easier and faster if I ran
the test suite from the beginning. Nevertheless, this is how I went about 
fixing the code. I ran the test suite a couple of times and started correcting
things where they needed to be corrected. One of the errors I encountered 
using the test suite was the double ‘2’ value in the Card object.

Afterwards, I did what I had also done with the other modules and had a look 
through the code. I found errors like the King card being checked whether it
can always be discarded instead of the Queen card like this.

So, to summarise, the main strategies for detecting errors I used were: 
* reading the code 
* testing the program
* using the test suite.
