Brett Fedack
CS372 Summer 2015
Project 2

NOTE:   This program was tested on OSU's flip servers.

Basic Instructions

    (1) Run ftserver on given port.
    (2) Run ftclient by passing the IP address and port number of ftserver,
        list (-l) or get (-g) command, filename, and data port.
    (3) Repeat (2) for additional FTP requests, or send SIGINT to
        terminate ftserver.

ftclient

    usage: python2 ftclient <server-hostname> <server-port> -l|-g
                            [<filename>] <data-port>

        <server-hostname> - IP address of server (dotted-quad or domain name)

        <server-port>     - port to bind with FTP control connection
                            endpoint; must be in range [1024, 65535]

        -l|-g             - file listing (-l) or file transfer (-g) command

        <filename>        - file to transfer from server to client

        <data-port>       - port to bind with FTP data connection
                            endpoint; must be in range [1024, 65535]

ftserver

    Run 'make' command to build the program.

    usage: ftserver <server-port>

        <server-port>     - port to bind with FTP control connection
                            endpoint; must be in range [1024, 65535]

Example

    FTP SERVER
    ---------------------------------------------------------
    FTP CLIENT

Sources

    Wikipedia - File Transfer Protocol

      https://en.wikipedia.org/wiki/File_Transfer_Protocol

    Beej's Guide to Network Programming

        http://beej.us/guide/bgnet/output/html/multipage/index.html

    Python 2 API

        https://docs.python.org/2/library/socket.html
        https://docs.python.org/2/library/struct.html
        https://docs.python.org/2/library/stdtypes.html#bltin-file-objects

    K&R C Section 8.6

    I adapted some of my code from project 1 for use in this project. No
    other code was borrowed; any similarities are purely coincidental.
