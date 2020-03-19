# Environment Variables in bash


This class is on Environment Variables


### What is an environment variable

variable is like a box, you can extract and put things inside and give it a name,

For us, an Environment is a system where code runs for different purposes.
Usually, at least these 3 environments exist:
- Development
- Testing
- Production

Environment variables are variables that exist in said environments and are interpolated from the environments and not from the code.

**environment variables exist in the machine and not the code.**

This is great for things:
- Things that you don't want to have in your code
- Like access keys
- Like AWS_SECRET keys
- Similar to SSH keys, the never go in the code, or even close

Allows us to keep them secret and they don't end up on GitHub where some wannabe hacker is going to find them and mine BitCoin



## Commands:
Printing in Python is the same as echo in bash

- echo MY_VAR
  - will print 'MY_VAR'

You can set the variables to do something

$ is an interpolation syntax. Similar to f' in Python

- MY_VAR=$(pwd)
  - now if you did echo $MY_VAR, it will print out the pwd


- If you restart the Terminal, it will no longer know what MY_VAR is because it is a new session.


### Bash child processes and exporting
- ./filename
  - runs a file inside a directory
