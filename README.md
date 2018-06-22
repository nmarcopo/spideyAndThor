# Systems Programming Final Project: Spidey and Thor
Originally Submitted to professor [Peter Bui](https://www3.nd.edu/~pbui/) on May 5, 2018.

# Addendum:
## TL;DR: compile with `make` and run with ./spidey. Navigate to localhost:[port] in your web browser
This project was absolutely ridiculous. Professor Bui's lectures on HTTP, TCP, etc. seemed simple enough, but when it came down to actually doing this project, all the concepts seemed so primitive compared to what we did. Thanks to all the TA's for their helpful hints, my classmates for their high level assistance, and Professor Bui for causing my group to skip studying for finals to complete this project on time.

# Original Readme:

Members
-------

- Nicholas Marcopoli (nmarcopo@nd.edu)
- Austin Sura        (asura@nd.edu)
- Sung Hyun Shin     (ssin1@nd.edu)

Demonstration
-------------

https://docs.google.com/presentation/d/1uxEwSPMoKRkB-4QWyqDZbSC5ZflS22lFqh5QLrLZA94/edit?usp=sharing

Errata
------

Summary of things that don't work (quite right).

We are aware that we fail one test to correctly mime-type .html. We fail to this because we think some default mime-type is being incorrectly put in, but we could not locate the source of this problem. We also have a problem in forking with valgrind leaks, but the forking valgrind test does pass all of the test_spidey.sh tests. When using forking, we also found that the server does not auto close itself once the tests are over, and we think that stems from either a while(true) loop or from previous valgrind erros.

Contributions
-------------

Enumeration of the contributions of each group member.

We all met together to work on the project in the same space and time. We had different emphasis on different functions, but we were all aware of what the files and functions do and how we were going to accomplish it. We were all collaborating and helping each other. 
Sung Hyun Shin focused on socket.c, single.c, accept_request, parse_request_headers,handle_request,handle_browse_request,handle_error,single.c, and functions in utils.c. Austin worked on thor.py, parse_request_method, parse_request_headers, handle_browse_request,handle_cgi_request,forking.c,spidey.c, and functions in utils.c. Nicholas worked on thor.py, accept_request, parse_request_method, parse_request_headers, handle_request, handle_browse_request,handle_browse_request,handle_error,forking.c,spidey.c,and functions in utils.c.
For debugging we all worked together and collaboratively to fix problems together.
