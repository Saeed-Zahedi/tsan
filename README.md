for Printing the Instrucions I have changed the MemoryAccess and MemoryAccess16 in "tsan_rtl_access.cpp".
when  the Accesstype is kAccessRead it prints the Instructions.
pc is the program counter and the size is the size which we are going to Access from Memory.
 
to print the mutex addresses and the pc which is locked I have changed the "tsan_interceptors_posix.cpp".
this file contains Interceptors based on the mutex actins like lock,unlock,init,... .it has pointer to mutexes and the pc so It conits all the things I need. 
