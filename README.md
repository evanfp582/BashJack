# BashJack
Blackjack written using bash scripts

Give your linux machine access to execute a bash script by running   
`chmod +x BashJack`  
while in the repo

Executed with ./BashJack  

### Debug mode  
DEBUG=1 ./BashJack  

## With a UI Intended Use
UI=1 ./BashJack  

### UI
<img width="1890" height="973" alt="image" src="https://github.com/user-attachments/assets/2a2dcf6f-6642-4bf8-b24f-93ff0cb3e769" />


### Minimum screen size 65x43
<img width="531" height="652" alt="image" src="https://github.com/user-attachments/assets/ed0d1899-dfe7-430b-9562-f5d58504c977" />


## At this point, unless you are a curious developer, this is unimportant 

# Learning Journey
First of all, I know that bash is not really meant to be used in this way.  
A more traditional programming language would have been far more 'effective' at doing this, but they joy is in the journey. not the destination  
I am learning a whole lot about bash from this project 

You can't return values like how you expect, the return is a status code  
You can return things by just echo'ing what you want to save and capturing it in a variable  
You **can** return things like how you expect by using the life saving local -n variable declations  
- Since finding out about these it made my project possible so I am actally able to do what I want
Scope can and will get in your way, which is why I do not mess with the sub-terminals    
Arrays are finicky, fail in unexpected ways, and like to become strings rather than arrays 

My entire experience changed once I learned about "local namerefs" in bash.  
As soon as I learned how to pass things are reference, I was no longer restrained to a really bad function system and being in `scope` hell.  

I learned that if something is working unexpectedly, more offen than not, it is a scope issue. Without a coprehansive debugger that can differentiate scope and global varaibles it because quite difficult to debug.  
I often resorted to just changing variable names even when it was not needed to rule that out as a possiblity.

## Overall
I learned that Bash can do some really powerful things and some really visually interresting things, but it is NOT a conventional programming language. Many of the conventions I have grown to love become a hastle or requiring and newish workarround to achieve.  
By doing this project I have learned much of the basic and fun that bash has to offer. I will continue to use bash scriping and vim more and more in both person projects and at work (Managing RHEL Server)


# TODO (Out of date, keeping for fun)
## Essential rules
- Aces being either 1 or 11 DONE  
- Split (I think this is going to be real difficult, perhaps not even worth doing tbh)
- Double DONE  
- Correct BlackJack payout (3-2 rather than 1-1) DONE

## User Interface
I have not fully decided what I want to do.  
I think a minimal TUI could be fun and easy enough, but even if I do not want to do that, the current commandline UI needs to be updated 


Working on the UI now!
<img width="938" height="970" alt="image" src="https://github.com/user-attachments/assets/60922786-94dd-4d9d-81a6-4cccbd106607" />
it is in a good state, but the data is all dummied out, adding the UI and gameplay together may be a bit painful


This is done and I am pretty happy with the state that it is in!

## Multiple Players
Allow for multiple people to be sit at the table with the user.  
I think it would be really cool to give them **play styles**
- The Card Counter
- Greedy
- Conservative  

I am not sure if/how I would want to implement this. It is one thing to try to implement this in the command line version of the program, but to add this to the UI seems a litle impossible due to space constraints.
So for the time being, no secondary player

I never did this due to challenges with viewing multiple hands at the same time (not to mention the logistic difficulty of adding multiple 'hands' and 'users' to a system designed for 1). The issue is bash does not really have a great way of dealing with arrays, so having more complex data objects (like a 2d matrix of 'hands') sounds like a real pain...   

# Resources
https://github.com/dylanaraps/writing-a-tui-in-bash 
