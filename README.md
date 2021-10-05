<b> Why Streams and I/O redirection ? </b>

Streams and Pipelines help us combine programs by sending the output of one program as the input to the next program. Pipes are executed on the terminal command line and are extremely useful.

As data scientists, we constantly work with large files. Pipes help us quickly understand the contents of a file without having to build programs and setting up a development environment like Jupiter. They are also easy to write as they are usually just one line.

Pipes also don’t depend on having python, anaconda or specific python packages installed on a system. They are executed directly by the shell. Another advantage of pipes is, they execute much faster than python scripts.

<b> Every UNIX process has four key components: </b> <br>
* a current working directory
* standard input(keyboard)
* standard output(terminal/screen)
* standard error. 

<b> Input/Output Redirection </b>

* Current working directory - It is the directory in your UNIX file system that you are currently at while running a command. All commands are executed relative to this directory. 
* Standard input - The standard input stream which provides inout to the commands. By default it is the keyboard.
* Standard output - the standard output stream displays the output from the commands. By default , it is the terminal screen/monitor.
* Standard error - The standard error stream displays error output from the commands when executed.

In a typical UNIX interface, the commands are entered with the keyboard and the ouput is displayed on the screen. Using redirection, we can change where the standard input comes from or where the output goes into.
This is accomplished using a reidrection operator which allows the user to specify the input or output data to be redirected to or f4om the file.

<b> Below are the most frequently used redirection operators: </b>

* <b> Pipe ' | ' </b> -  This operator sends the output of one program as the input to another for processing. It connects two processes and the output of the first process does not get displayed on the screen. It is useful for parallel processing of the commands.<br>
      The general syntax looks like - command_1 | command_2 | command_3
      
* <b> Output Redirection ' > ' </b> - This operator directs the output of a program/command executed to a file entered after it. If the file aready has some components present, they get over written with the new commands' output.<br>
      The general syntax looks like - command > output_file_spec
      
* <b> Input Redirection ' < ' </b> - This directs standard input to a process for execution.<br>
      The general syntax looks like - command < input_file_spec
      
      
To append the output of a command executed to an exisitng file without overwriting it, we use ' >> ' operator.


To execute UNIX commands in jupyter environment(jupyter notebook), we add a ' ! ' symbol at the beginning of each executable command.


For more details and examples, please refer <a href='https://github.com/Tansha173/I-O_Redirection/blob/master/I:O_Redirection.ipynb'>Input-Output_Redirection</a>

