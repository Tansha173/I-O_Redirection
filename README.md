
<b> Why Streams and I/O redirection? </b>

Streams and Pipelines help us combine programs by sending the output of one program as the input to the next program. Pipes are executed on the terminal command line and are extremely useful.

As data scientists, we constantly work with large files. Pipes help us quickly understand the contents of a file without building programs and setting up a development environment like Jupiter. They are also easy to write as they are usually just one line.

Pipes also don’t depend on having python, anaconda, or specific python packages installed on a system. They are executed directly by the shell. Another advantage of pipes is that they execute much faster than python scripts.

<b> Every UNIX process has four key components: </b> <br>
* a current working directory
* standard input(keyboard)
* standard output(terminal/screen)
* standard error. 

![25659271-E900-464B-8E04-1BCC9DE7A6AD](https://user-images.githubusercontent.com/83805469/137371505-f3a77d45-89f3-43d2-bafc-643bc920d3ba.png)

<b> Input/Output Redirection </b>

* Current working directory - It is the directory in your UNIX file system that you are currently at while running a command. All commands are executed relative to this directory. 
* Standard input - The standard input stream which provides input to the commands. By default, it is the keyboard.
* Standard output - the standard output stream displays the output from the commands. By default, it is the terminal screen/monitor.
* Standard error - The standard error stream displays error output from the commands when executed.

In a typical UNIX interface, the commands are entered with the keyboard and the output is displayed on the screen. Using redirection, we can change where the standard input comes from or where the output goes.
This is accomplished using a redirection operator which allows the user to specify the input or output data to be redirected to or f4om the file.

<b> Below are the most frequently used redirection operators: </b>

* <b> Pipe ' | ' </b> -  This operator sends the output of one program as the input to another for processing. It connects two processes and the output of the first process does not get displayed on the screen. It is useful for parallel processing of the commands.<br>
      The general syntax looks like - command_1 | command_2 | command_3
 
      
* <b> Output Redirection ' > ' </b> - This operator directs the output of a program/command executed to a file entered after it. If the file already has some components present, they get overwritten with the new commands' output.<br>
      The general syntax looks like - command > output_file_spec <br>
      To sort the contents of a file, foo.txt, and save its output to sorted_foo.txt, we execute the following command - <br>
      
      sort foo.txt > sorted_foo.txt
      
* <b> Input Redirection ' < ' </b> - This directs standard input to a process for execution.<br>
      The general syntax looks like - command < input_file_spec <br>
      To send a file as an input to the command sort, like above, we execute the following command - <br>
            
      sort < foo.txt > sorted_foo.txt
      
      
To append the output of a command executed to an existing file without overwriting it, we use the ' >> ' operator.


To execute UNIX commands in jupyter environment(jupyter notebook), we add a ' ! ' symbol at the beginning of each executable command.


For more details and examples, please refer <a href='https://github.com/Tansha173/I-O_Redirection/blob/master/I:O_Redirection.ipynb'>Input-Output_Redirection</a>

