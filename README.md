# BashJack
Blackjack written using bash scripts


# Learning Journey
First of all, I know that bash is not really meant to be used in this way.  
A more traditional programming language would have been far more 'effective' at doing this, but they joy is in the journey. not the destination  
I am learning a whole lot about bash from this project 

You can't return values like how you expect, the return is a status code  
You can return things by just echo'ing what you want to save and capturing it in a variable  
You **can** return things liek how you expect by using the life saving local -n variable declations  
- Since finding out about these it made my project possible so I am actally able to do what I want
Scope can and will get in your way, which is why I do not mess with the sub-terminals    
Arrays are finicky, fail in unexpected ways, and like to become strings rather than arrays 


# TODO
## Essential rules
- Aces being either 1 or 11
- Split (I think this is going to be real difficult)
- Double
- Correct BlackJack payout (3-2 rather than 1-1)

## User Interface
I have not fully decided what I want to do.  
I think a minimal TUI could be fun and easy enough, but even if I do not want to do that, the current commandline UI needs to be updated 

## Multiple Players
Allow for multiple people to be sit at the table with the user.  
I think it would be really cool to give them **play styles**
- The Card Counter
- Greedy
- Conservative  

# Resources
https://github.com/dylanaraps/writing-a-tui-in-bash 
