## Handling concurrency
1. 3 ways of handling
	1. Threading
		1. Threading is generally faster than threads because it is all within the same namespace but if one of them crashes then the whole program crashes
	2. Processes
		1. Processes spawn other processes so therefore if one of them crashes critically they can continue on their own 
	3. IO preprocessing
		1. In C the process of binding on the server is the following
			1. Socket
			2. Bind
			3. Listen 
			4. Accept
		2. On the client side C process binding processes
			1. Socket
2. Different types of returns for multiplexing IO
	1. select
	2. poll
	3. epoll 
	4. kqueue
3. This is for any process that returns a file descriptor 
