Context switching 
My context switching is preformed by an assembly routine thread_switch.s that saves the current thread's stack pointer and transfers control to the next thread. Threads explicitly give control in thread_yeild.

Limitations
the max amount of threads is fixed at 16 and each thread uses 4096 bytes of stack. Since it is cooperative, a thread that doesnt yeild can block the entire system. There is also no priority or order in the scheduler.