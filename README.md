LBE-OperatingSystem
===================

LBE-OS is a repo full of code snippets to help you complete your OS labs. 

A few things to point out :
- Though I did my best, I might have done some mistakes along the way, [let me know](https://github.com/Diastro/LBE-OperatingSystem/issues) AND/OR contribute to fix them!
- Think there would be more interesting things to add in there, feel free to add them OR request that I do a quick example.
- Without sharing, we won't go anywhere! Contribute! Go Open! Drink tea.

*David Albertson*

##Execution
To run any code example in a Linux environment (I use ubuntu) do the following :

1) Compile any .cpp file :
    
~~~ sh
gcc 01fork.cpp -o output
~~~
    
For the **Thread** section you need to add the `-pthread` flag
  
2) Execute the corresponding output file :

~~~ sh
./output
~~~
    
##Content

### Process

* Basics
    * **01fork.cpp** - Creating a new process
    * **02waitpid-basic.cpp** - Wait for a given process to terminate
    * **02waitpif-elaborated.cpp** - Wait for a given process to terminate and retrieve signal or exit value
    * **03waitpid-nonBlocking.cpp** - Wait for a given process to terminate without blocking the parent process
    * **04wait.cpp** - Wait for all process to terminate
* Execution
    * **01execve.cpp** - Replacing the child process image by a new one
    * **02execlp.cpp** - Replacing the child process image by a new one
    * **03execvp.cpp** - Replacing the child process image by a new one
    * **04exec-example.cpp** - Replacing the child process image by a new one using a user created executable
    * **05execWait-example.cpp** - Replacing the child process image by a new one and wait for the child process to terminate before terminating the parent process
* IPC
    * **01pipe.cpp** - Communication using a pipe and file descriptors (parent process writing to child process)
    * **02pipe-interProc-basic.cpp** - Communication between 2 process using a pipe and file descriptors
    * **02pipe-interProc-elaborated.cpp** - Communication between 2 process (using a user created executable and passing fd as arguments)
    * **03pipe-twoWayComm.cpp** - Communication using a pipe and file descriptors (two way communication)

### Threads

* Basics
    * **01thread.cpp** - Launching threads for specific task
    * **02thread-arguments.cpp** - Passing arguments to threads
    * **03thread-multipleTask.cpp** - Clean way of launching multiple threads
* Synchonization
    * **01mutex.cpp** - Basic synchonization using mutex (binary semaphores)
    * **02semaphore-prodCons.cpp** - Synchronization using semaphore. An example of the producer - consumer problem
    
##Changelogs
TOD.

FIFO coming soon.

##References
- [Die.net - Linux Doc](http://www.die.net)
- [A short introduction to operating systems, by Mark Burgess](http://www.iu.hio.no/~mark/os/os.html)
- [Google's CPP coding guideline](http://google-styleguide.googlecode.com/svn/trunk/cppguide.xml)
