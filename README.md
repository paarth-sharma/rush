# Rush

# What is Rush ?
My attempt at creating a basic rust-based shell prompt

# Basics

## What is a Shell ?
A shell is a program which allows you to control your computer. It does this largely by making it easy to launch 
other applications. But a shell on it’s own isn’t an interactive application, so use an application called a
terminal emulator to interact with it.

## Starting point
At the very least, the simplest interactive program must be able to take user input

- [x] Taking user input

## Accepting multiple commands
The shell doesn't stop taking commands till terminated, so it should be able to take multiple commands from the user. The way to do it, is to input the command to take inputs in an infinite loop and to set constraints(s) to break out of it if and when the user so wishes.

- [x] Accept multiple commands

## Handling args
An argument is the input given to a command line to process, with the help of which is can process it better
eg:
- giving the source and child directories
- passing file/directory names
In order to precisely execute a command and make sure it does the intended job, passing and handling args is neccessary

- [ ] Handling arguments of a command

## Shell builtins
Having a set of pre-set commands, programmed to carry out specific tasks is very usefull for 2 reasons -
<ol>
    <li>It saves time; you can bind lengthy commands to smaller keywords by setting them as aliases</li>
    <li>often more intuitive to type them, rather than to commit large instructions to memory</li>
</ol>

eg:
- `` cd `` is a common shell builtin that hepls navigate to directories, which is vital fucntionality 
- `` ls `` command that helps find out what directories contain and so on.

- [ ] Adding some built-in commands for the shell, like all other shells

## Error-handling
If you’ve worked with shells, you will notice that they don't crash if you input a command which does not exist, instead they print a meaningful error message which can be used to identify the problem the caused the crash. In my implementation below, that is handled by printing an error to the user and then allowing them to enter another command.

- [ ] Error handling

## Pipes
It would be difficult to be productive in a shell which didn’t include pipes. If you aren’t familiar with this feature, the 
``
|
`` character is used to tell the shell to redirect the output of the first command into the input of the second command. 
For now the shell includes a very basic support for pipes.

- [ ] Piping output of one function into other functions using `` | `` symbol