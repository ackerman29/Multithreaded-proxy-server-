# THE NEED FOR THIS PROJECT #
To Understand →
The working of requests from our local computer to the server.
The handling of multiple client requests from various clients.
Locking procedure for concurrency.
The concept of cache and its different functions that might be used by browsers.
Proxy Server do →
It speeds up the process and reduces the traffic on the server side.
It can be used to restrict user from accessing specific websites.
A good proxy will change the IP such that the server wouldn’t know about the client who sent the request.
Changes can be made in Proxy to encrypt the requests, to stop anyone accessing the request illegally from your client.

# OS COMPONENTS USED ​#
Threading
Locks
Semaphore
Cache (LRU algorithm is used in it)

# LIMITATIONS ARE #
If a URL opens multiple clients itself, then our cache will store each client’s response as a separate element in the linked list. So, during retrieval from the cache, only a chunk of response will be send and the website will not open
Fixed size of cache element, so big websites may not be stored in cache.

# HOW TO RUN #
In your terminal : ./proxy "port number"
Open http://localhost:port "portnumber"/https://www.cs.princeton.edu/

# WORKFLOW #
<img width="601" alt="Screenshot 2024-07-07 at 1 55 04 PM" src="https://github.com/ackerman29/Multithreaded-proxy-server-/assets/104158912/a3c11380-dfd4-482b-b3f3-dd8ca91318c6">

# SCREENSHOTS #

<img width="756" alt="Screenshot 2024-07-06 at 3 21 02 PM" src="https://github.com/ackerman29/Multithreaded-proxy-server-/assets/104158912/4e7bcb33-59f4-4b88-9359-c92667115bab">
<img width="862" alt="Screenshot 2024-07-06 at 3 21 17 PM" src="https://github.com/ackerman29/Multithreaded-proxy<img width="906" alt="Screenshot 2024-07-06 at 3 22 40 PM" src="https://github.com/ackerman29/Multithreaded-proxy-server-/assets/104158912/0eea4aae-2489-44c6-8b6a-58dcd530f945">
-server-/assets/104158912/5db64bfa-640a-4d0e-8989-2fb44a6f94f9">

<img width="886" alt="Screenshot 2024-07-06 at 3 23 57 PM" src="https://github.com/ackerman29/Multithreaded-proxy-server-/assets/104158912/a22a76db-ef3e-4b38-b29b-4468569b56ac">

# NOTE #
This code can only be run in Linux Machine. Please disable your browser cache.(TRY INCOGNITO MODE)
To run the proxy without cache Change the name of the file (proxy_server_with_cache.c to proxy_server_without_cache.c) MakeFile.



