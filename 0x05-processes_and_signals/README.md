0x05. Processes and signals

What is a Process?
A process can be thought of as an instance of a program in execution. We called this an ‘instance of a program’, because if the same program is run lets say 10 times then there will be 10 corresponding processes.

Moving ahead, each process has its own unique process ID through which it is identified in the system. Besides it own ID, a parent’s process ID is also associated with a process.

The main() Function
A ‘C’ program always starts with a call to main() function. This is the first function that gets called when a program is run.

The prototype of a main() function is :
int main(int argc, char *argv[]);
#include<stdio.h>

int main(int argc, char *argv[])
{
  int count = argc;
  printf("\n The number of arguments passed is [%d] \n", count);

  int c = 0;
  while(c < count)
  {
    printf("\n The argument [%d] is : [%s]\n", c+1, argv[c]);
    c++;
  }
  return 0;
}

Signal	Description
SIGHUP	Hang-up detected on controlling terminal or death of controlling process.
SIGINT	Issued if the user sends an interrupt signal (Ctrl + C).
SIGQUIT	Issued if the user sends a quit signal (Ctrl + D).
SIGFPE	Issued if an illegal mathematical operation is attempted.
SIGKILL	If a process gets this signal, it must quit immediately and will not perform any clean-up operations.
SIGTERM	Software termination signal (sent kill by default).
SIGALRM	Alarm clock signal (used for timers).
When executed on the terminal, the command

man 7 signal 
