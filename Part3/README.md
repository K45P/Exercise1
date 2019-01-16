# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 Concurrency is when a computer solves tasks at the same time, but the tasks are independent of each other. Paralellism is when a computer solves a single task while using multiple processes at the same time.
 
 ### Why have machines become increasingly multicore in the past decade?
 >The clock speed of processors became hard to increase, so instead of having one processor executing all the tasks, the tasks are split between multiple cores to increase efficiency.
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > problems that have many different machines and problems that need solving independently
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *Your answer here*
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > tgreads are the smallest possible instruction set that can be managed independently. A process is the combination of computer code and the activity of a computer program being executed. Green threads can be seen as user made threads that are managed by an ordenary process, instead of by the operating system. Coroutines are functions that can be paused and started before returning. This means that when two or more functions have a coroutine, one function can affect the other function without returning to it.
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > In go it will make a goroutine. in python it creates a thread. In c it creates a thread
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > it prevents multiple threads from executing at once.
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > using another interpreter, such as jpython??
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > *sets the maximum number of processors that can execute simultaneously. 
