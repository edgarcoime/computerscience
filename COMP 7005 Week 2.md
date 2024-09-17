### File Descriptors
1. In a process there is an array of file descriptors
2. FDS
	1. foo < in.txt
		1. Replaces 0/stdin with in.txt
	2. > out.txt
		1. Replaces 1/stdout with out.txt
	3. 2 > err.txt
		1. Replaces 2/stderr with err.txt
3. Any further FDS that are opened up will take up the next available slot in the FDS array 
4. File descriptors are able to 
	1. close
	2. read 
		1. Take a file descriptor FD, buffer buf, and size 5
		2. read can return the following
			1. -1, 0, 1 -> n (where n == 5 in this case)
			2. -1 error
			3. 0 successful 
				1. 0-n shows what parts of the value were able to be read 
	3. write
		1. Take a file descriptor FD, buffer buf, 5
		2. write can return the following
			1. -1, 0, 1 -> n (where n == 5 in this case)
			2. -1 error
			3. 0 successful 
				1. 0-n shows what parts of the value were able to be written 
5. Ring Buffer
	1. Think of it like a cyclic array
	2. a -> b -> c -> d -> e -> f
	3. Can read from 
6. When applied to packets
	1. A packet can store 1500 
	2. If we needed 1501 then it would send a second packet with just 1 bit of data
7. With regards to interacting with files on the disc you can have these file descriptors
	1. open: is to open a file
	2. creat: is to createa. file
	3. dup:
	4. dup2
	5. socket
8. With sockets you can have
	1. IPC: Inter process communication
		1. Domain/unix socket
		2. uses a /path
	2. Network communication or remote communication
		1. network socket
		2. uses an IP address with port 
9. Communication using client server in an IPC
	1. A client connects to the server using IPC network in an TCP connection
		1. Server:
			1. process:
				1. socket
				2. bind
				3. listen
					1. Listen sets up socket so that it can accept connections
				4. accept (intercepts connect request from client)
				5. read/write
				6. close
			2. FDS:
				1. in
				2. out
				3. err
				4. f
		2. client:
			1. process
				1. socket
				2. bind (optional usually doesn't)
				3. connect (server has to accept connection)
				4. read/write
				5. close
			2. FDS:
				1. in
				2. out
				3. err
				4. fd
10. Simple server example through pseudo code
```c
socket
bind
listen
while(true)
{
	fd = accept();
	process(fd);
}
```
11. There are different ways to handle sockets
	1. Multiplexing I/O (covering this one in this course)
	2. threads
	3. process
12. Domain sockets
	1. Client and server will all be in 1 computer
	2. Client will ask for filename nd server will give it the file contents