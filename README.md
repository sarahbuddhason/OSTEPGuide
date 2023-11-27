## Process API

- Create new process with pair of system calls: fork(), exec()
- A process can use wait() to wait for a process it has created to complete

### fork()

- fork() is used to create a new process, which is an almost exact copy of the calling process.
- The child process starts executing from the point of the fork() call, not from the beginning of the program.
- After fork(), there are two processes in execution: the parent and the child.
- The parent receives the process identifier (PID) of the child, while the child gets a return value of zero.
- The behavior of the CPU scheduler makes the execution order of the parent and child non deterministic.

### 
