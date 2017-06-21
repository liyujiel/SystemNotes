# SystemNotes

### Difference between forking and multiThereading 

A for give us a brand new process which is a copy of the cureent process with the same code segment. it looks exactly like the parent process with different process id having it's own memory. Parent process creates a separate address space for the child with same code segments but executes independently of each other. Because the system issues a new memory space and enviroment for the child process, it is knows as heavy-weight process.

While thread can execute in parallel with same context. Also memory and other resources are shared between the thread casuing less processes as they don't have any overhead as compared to processes(as it doesn't issue any separate command for creating completely new virtual address space). A single process can have multiple thread. For all threads of any process, communication between them is direct. While process needs some interprocess communication mechanism to talk to other processess. Thought, thread seem to be more usefor for any reason, do notes that changes in any thread may lead to changes in other threads of the same process. While, change in child processes is independent as parent process has its own execution copy.
