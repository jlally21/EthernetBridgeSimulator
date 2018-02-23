# CS3700 Project 2 Simple Bridge

Our high level approach to implementing a bridge program largely followed the project description:
First, we set it up to just read from and write to sockets with incorrect information. We then moved on
to building the spanning tree, followed by forwarding data packets. Once we had this mostly working, we improved
the implementation to handle new and failed bridges.

Most of our time was spent building the spanning tree. While it didn't take too long to get a semi-working
spanning tree protocol, we faced many challenges in getting all edge cases to work. Specifically, setting both
designated bridges for LANs and setting designated ports when a bridge has multiple ports going to the same LAN.
We ended up drawing many configurations on paper to help us decide what ports should be active and what ports
should be inactive, and eventually had a solid spanning tree protocol implementation.

Our code was tested primarily through the use of the 'run' and 'test' scripts. When we found failing tests,
we would go in and run individual configurations with debug statements and changes to investigate and fix
our edge case failures.
