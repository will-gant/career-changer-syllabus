# Syllabus

## Computer science

- [ ]  Understand that fundamentally computers execute *instructions* on *data*
- [ ]  Understand that ultimately a computer’s processor, or CPU, *just does maths* - specifically, addition and subtraction (all other types of maths just combine these two operations).
- [ ]  Read up on the base-2 (or “binary”) counting system, and understand how it differs from the base-10 counting system (”decimal”) humans use.
    - [ ]  Note that if binary represents instructions in a compute program (rather than, say, the data stored in a file) it can be referred to as “*machine code”*.
    - [ ]  Without using a computer, convert the following base-10 numbers into base-2/binary: `5`, `42`, `246`
- [ ]  Understand that all data computers store, read, write and process is binary. Reflect on the implication of this - that all electronic files, programs, etc are just ******************very, very large numbers******************.
- [ ]  Read into a few basics on bits and bytes, but don’t go crazy…
    - [ ]  Understand that a ‘bit’ is the smallest unit of information, representing a 1 or a 0. On or off. True or false.
    - [ ]  Find out how many ‘bits’ are in a ‘byte’, and how many of each are needed to ‘encode’ a single character on your keyboard using “[ASCII](https://en.wikipedia.org/wiki/ASCII)”
    - [ ]  Work out how many bits and bytes are needed to store your first name. Optional: spell out your first name in binary.
- [ ]  Briefly dip your toe into some beginner-level material on CPU *instruction set architectures*.
    - [ ]  Understand that an instruction set, in this context, basically defines the particular binary instructions that can be used to tell a CPU what to do.
    - [ ]  Find out what kind of popular devices tend to have 'x86-64' CPUs, and which ones usually have have 'ARM' CPUs.
- [ ]  Find out the name of the most ‘low-level’ language that we have *other than* binary. Don’t bother trying to learn any of its syntax - but do try and find a simple example of a ‘hello world’ app written in this, just for a flavour of what it looks like.
- [ ]  Find some beginner-level material to read on what happens when a computer starts running a program (what is the role of memory, i.e. “RAM”?)
- [ ]  Find out the basic distinction between “binary” files and text files (note that confusingly both are, in fact, stored as binary)
    - [ ]  Understand that the binary content of ‘text files’ can be ‘[decoded](https://en.wikipedia.org/wiki/Character_encoding)’ into human-readable text. Any file you can read in your text editor is a ‘text file’, regardless of file extension.
    - [ ]  Illustrate to yourself that the binary of “binary” files can’t be decoded this way. Find a binary file on your machine (e.g. an image or a PDF), and open it in a text editor. Marvel at the garbled nonsense.
- [ ]  Understand that a computer program whose instructions are stored in text files - e.g. a `.rb` file containing ruby code - is referred to as “source code”. And that source code must be translated into machine code before a computer can execute it.
- [ ]  Read up on the distinction between:
    - [ ]  Running a program from source code with an ‘interpreter’
    - [ ]  Running a program from an executable binary file that has been ‘compiled’ from source code

> **_Field trip:_** If you live in the UK, go to the [National Museum of Computing](https://www.tnmoc.org/) in Bletchley (near London). Pay extra to book on a guided tour, and allow at least three hours. Your guide will be a true afficionado - likely a retired software or electronics engineer - and you'll learn bucketloads about computing fundamentals.

## Operating systems

- [ ]  Understand the basic definition of an OS
- [ ]  Understand the relationship between an OS and a *****shell*****
- [ ]  Look up the definition of a ***********system call***********
- [ ]  Understand that shells and programming languages are often used to make ************system calls************
    - [ ]  Understand that a significant proportion of what most software does consists of asking the OS to do stuff via system calls.
    - [ ]  Understand that the exact system calls available vary by OS, and therefore at some level some sort of ‘translation’ is needed to get software written for one OS to run on another
- [ ]  Understand what a ‘GUI’ is, and that your operating system’s GUI is just a computer program running on top of your OS (just like a shell). Most of what you can do in a GUI can be done in a shell, and vice-versa - they’re different tools for making the exact same system calls.
- [ ]  Understand that more than 90% of servers in the world run some form of Linux, and that Windows and macOS are increasingly for personal computers
- [ ]  Make the same system call to create empty files in the same directory in three different ways:
    1. By clicking buttons using your operating system’s GUI
    2. Running a shell command
    3. Writing some code to use one or more methods from ruby’s ‘standard library’ to create the file
- [ ]  Understand that an OS usually has a particular **********filesystem********** - i.e. a structure it uses for organising directories, files, etc
    - Find out what the ‘top’ level of the file system is on a Windows machine
    - Ditto for a Linux machine (don’t worry about Linux ‘distributions’ at this stage)
- [ ]  Don’t worry about the details, but understand that a single physical machine can use ****************virtual machines**************** to run multiple operating systems at the same time

## Shells and terminals

- [ ]  Learn the name(s) of the terminal, or terminals, your OS offers you out of the box.
- [ ]  Find out which shell you’re using by default in your chosen terminal
- [ ]  Find out the name of at least one other shell that you could use with your OS
- [ ]  Really important: make sure you understand the difference between a *****shell***** and a terminal
- [ ]  Understand that if you see the term ‘terminal emulator’, it just means a terminal (originally ‘terminal’ referred to a big physical machine in an office that was dedicated to running a shell)
- [ ]  Understand that shells are not necessarily tied to operating systems and some (e.g. `bash`) have versions that can run on many different types of OS.
    - [ ]  Make sure you understand that a shell that’s available on different types of OS might present the ****user**** the same interface, but is making different system calls under the hood
- [ ]  Make sure you’re comfortable doing the following from your terminal:
    - [ ]  Changing directory
    - [ ]  Printing out your current ‘working’ directory
    - [ ]  Creating a file
    - [ ]  Creating a directory
    - [ ]  Copying each of the above (including copying the *contents* of a directory along with the directory itself!)
    - [ ]  Deleting each of the above
    - [ ]  Printing out the contents of a human-readable file (e.g. a `.rb` file) in the terminal
    - [ ]  Starting your text editor and loading the files in the current directory

### Running programs from a shell

- [ ]  Learn what an environment variable is.
- [ ]  Set an environment variable, print its value, and then unset it.
- [ ]  Learn what your PATH is, and how your shell uses it when you try to run programs
- [ ]  Understand the difference between
    - Running a built-in command of your shell (e.g. `cd` to change directory)
    - Using your shell to run a separate program whose filepath is in your PATH
- [ ]  Understand that a program you run from your terminal is often referred to as a ‘command-line interface’, or CLI
- [ ]  Understand that most programs allow users to provide *******configuration******* in one of these forms:
    - An specific environment variable set to a certain value
    - A configuration file saved with a specific name/in a specific place
    - Command line ‘arguments’ or ‘flags’ that you include when you run the program

### Scripting

- [ ]  Understand that the commands of a shell are another language, just like ruby
- [ ]  Understand that anything you run in a terminal is something you can write in a file as a ******script******
- [ ]  Write the simplest possible ‘hello world’ shell script in a file and run it from your terminal

## Networking

- [ ]  Understand that all computers on a network have an **********IP address**********, which is like a postal address. As a postal address can theoretically be changed, so can an IP address.
- [ ]  Be aware that a distinction exists between:
    - ‘IPv4’ IP addresses (e.g. 192.168.0.1)
    - ‘IPv6’ IP addresses (e.g. 2001:db8::2:1) - a newer kind growing in popularity
- [ ]  Know the different purposes of public and private IP addresses, and understand one computer can, and usually does, have both simultaneously
- [ ]  Do the following:
    - [ ]  Find out your public IP address from your terminal
    - [ ]  Find out your private IP address from your terminal
- [ ]  Understand that in order to talk to each other computers need to know the IP address and ****port**** they need to send messages to
- [ ]  Understand the basics of ‘DNS’ - i.e. that web addresses translate into IP addresses, which is what your computer needs to actually send a message to a server
    - [ ]  From your terminal, find out what IP address [`www.example.com`](http://www.example.com) ‘resolves’ to
    - [ ]  Read up on what `[localhost](http://localhost)` is. From your terminal, find out what IP it resolves to.
- [ ]  Read a beginner-level introduction to HTTP
    - [ ]  Understand that your web browser makes ‘HTTP requests’ when you visit pages
    - [ ]  Learn how `GET`, `POST`, and `DELETE` requests are different (there are others, but don’t worry for now)
    - [ ]  Find out what port a web browser uses by default when visiting a website with HTTP
    - [ ]  Understand that there is a more secure version of HTTP called HTTPS. ************Do not worry************ about the details of how it works!
        - [ ]  Find out the default port a web browser uses when visiting a website with HTTPS.
- [ ]  Make a HTTP ‘GET’ request to [`http://httpbin.org/get`](http://httpbin.org/get)
    - [ ]  From your terminal (there are several different ways to do this)
    - [ ]  In a simple ruby program. This might be a little tricky for a total newbie - cheating is encouraged, and if it takes more than 30 mins feel free to skip.
- [ ]  Read a little about the ‘OSI model’, and see if you can figure out where HTTP fits into this. Don’t worry about understanding it all, or memorising it.

## Writing software

### General

- [ ]  Make sure you’re comfortable with the basic idea of what an application programming interface (API) is.
    - [ ]  Understand that an API can be used to allow a program written in one language (e.g. ruby) to ‘talk to’ a program written in a completely different language (e.g. python)
- [ ]  Find out what a software ‘library’ is (in the ruby world these are called ‘gems’) and why developers might want to use them.
    - [ ]  Take a look at the readmes of one or two popular ruby gems (e.g. [Devise](https://github.com/heartcombo/devise)) just to get a flavour of why a ruby developer might want to use them in their program
- [ ]  Don’t go deep, but read briefly about the difference between ‘dynamically-typed’ programming languages (like ruby) and ‘statically-typed’ ones (like Java).
    - The ‘types’ of variables (i.e. whether a variable is a string/integer/etc) must all be predetermined and consistent when a program written in a statically-typed language starts running
    - In ruby, etc the types are not checked until the program actually gets to that part of the code while it is running (”*at runtime*”), which allows flexibility but also makes mistakes more likely
- [ ]  Get familiar with the terms ‘unit tests’ and ‘test-driven development’ (”TDD”). Don’t bother actually learning how to use these yet.

### Clients and servers

- [ ]  Understand that a server is a program, usually running continuously, that ‘listens’ for messages from clients and then acts based on those messages
- [ ]  Understand the basic difference between a server and a client, including the fact that the same program can be a ‘server’ in one context and a ‘client’ in another.
- [ ]  Understand that a server is a program running on a computer, and not the computer itself
- [ ]  Banish the idea from your head that servers are necessarily something to do with websites or the web. Your computer will be quietly running several servers right now, used by ‘clients’ that are other programs on your machine.

### Data

- [ ]  Understand the broad concepts of an *****array***** (or ‘list’) and a ****hash**** (or ‘dictionary’/’map’) in ruby. Understand that these are universal concepts across programming languages, and are examples of ‘*data structures’*.
- [ ]  Understand that all data in a running computer program (e.g. the value of a variable) is stored *********in memory********* (i.e. RAM).
- [ ]  Understand that all memory is continually being pruned/reorganised, and gets wiped completely when we switch off our computer
- [ ]  Know that if we want to make sure our data *persists* when we switch off our computer, our program must generally store it in one or more files on a hard disk
- [ ]  Understand these options:
    - [ ]  Our program directly writes ordinary, human-readable text to a file on disk
    - [ ]  Our program asks a ‘database server’ to store data on disk for us in a database (usually in a format humans can’t read)
- [ ]  Understand that the most common kind of ‘database’ is a *******************relational database*******************, which stores data in tables with rows and columns - like a spreadsheet
- [ ]  Understand that ‘the database’ is a named group of such tables, stored in files on disk, and that one database server might have access to several unrelated databases.
- [ ]  Understand that databases often exist on a completely different computer from the program that wants to use them (but don’t have to be)
- [ ]  Understand that your program cannot interact with these files directly, and needs an intermediary - another program called a ‘*database server*’. E.g. *PostgreSQL* and *****MySQL*****.
- [ ]  Know that *SQL* is a universal language that both humans and computer programs can use to ask a relational database server to read from, and write to, a database.

### Version control

- [ ]  Learn what `git` is, and how it is different from [GitHub](https://github.com/)
- [ ]  Understand the *******purpose******* of version control - i.e. we ‘save’ our code regularly and can ‘revert’ back to earlier points in time if we want to.
- [ ]  Read a little bit about git ‘branches’ just to get a flavour of them. Don’t worry if you don’t fully get it.
- [ ]  Imagine the chaos that would exist if a team of developers tried to collaborate on the same code base ******without****** any kind of version control.
- [ ]  Register an account with github.com
- [ ]  Create a new repository with a readme, and ‘clone’ it to your machine
- [ ]  Follow GitHub’s [instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=windows) for creating an ‘SSH key’ (this is basically what lets you ‘authenticate’ with GitHub when running `git` commands in your terminal)
- [ ]  Use each of these commands at least once and get a very basic idea of what they do:
    - [ ]  `git add` (’stage’ changes to bits of code that I want to save)
    - [ ]  `git commit -m <commit message>` (’save’ changes to the bits of code I’ve staged)
    - [ ]  `git push` (upload commits to a remote repository - e.g. on GitHub)
    - [ ]  `git log` (look at previous commits)
    - [ ]  `git revert` (reverse a previous commit)
- [ ]  Create a new file in the repo, add and commit it, and then push it. Then verify you can see your change in github.com.
- [ ]  Then revert your commit and push again, and verify that you can see this in github.com

## Ruby

- [ ]  Know how to run `irb` so you can play around in the ruby shell from your terminal if you want to test something out
- [ ]  Assign values to variables
- [ ]  ‘Print’ data to the screen with `puts`
- [ ]  Write an `if` statement, and use `elsif` and `else`
- [ ]  Learn how to use arrays
- [ ]  Learn how to use hashes
- [ ]  Learn how to ‘loop’ over an array and do something for each thing it contains
- [ ]  Write a simple method
- [ ]  Understand the distinction between a method ******returning****** a value and printing that value with `puts`
- [ ]  Get your head around classes
    - [ ]  Understand that a class is like the technical schematics for a car, while an instance of that class is like an actual car made from those schematics
    - [ ]  Understand that instances of a class can hold data (attributes) and do stuff (methods)
    - [ ]  Write a very basic class with a simple method. Create an ‘instance’ of your class and call the method.
    - [ ]  Understand that classes are another concept that is common to many (not all) programming languages - not just ruby.
