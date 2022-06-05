# simple-webserver

to build and run a simple tcp server just use ncat. https://nmap.org/ncat/ 

This turns ncat into a simple web server. 
Continuing the example from the section called “A Listen Mode Example”, we can create a simple HTTP server that serves the index.html file using the following command:

	ncat -lk -p 8080 --sh-exec "echo -e 'HTTP/1.1 200 OK\r\n'; cat index.html"

Or, if you're a Windows user:

	ncat -lk -p 8080 --sh-exec "echo HTTP/1.1 200 OK& echo(&type index.html"

an index.html file is here 
