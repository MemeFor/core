# Data Mining Operations Spec
# Revision 0.01

## Summary

Herein described is the specification for a multi-user system to retrieve, parse, 
and organize data from internet communities to generate profiling, reports, and 
allow operational user-developers to refine these functions for the requests and 
requirements of clients and system hosts.

## System Requirements

The system is distributed to userbase, running the required programs on a Linux machine. 
The libraries included should be 32/64 bit OS agnostic and ideally cross-platform for
distribution to non-linux systems, though no scripts or tools for cross-compatability
 will be developed until needed.  The libraries required are as follows.

* PostgreSQL Database
* Steel Bank Common Lisp
* the required Lisp libraries, such as quicklisp
* GNU Emacs
* headless browser platform (TBD)

## System Operation

Userbase controls Emacs and Common Lisp runtimes atop hosts in communication 
with PostgreSQL databases, a unique database instance for each host. Requests 
are made from Emacs to query previous mining sessions for analysis, and to start
or setup new mining sessions on both local and remote hosts.

# Mining Sessions 

For mining sessions, user system runtime controls either a headless browser or make requests 
to webservers for data, as sessions recorded in database for a mining domain per host, either as 
a particular community board or multi-page crawl (TBD). Post content, post ID, poster/user IDs,
 post replies, and image or content URLs are stored in a relational database on each host. 


# To Be Decided

* headless browser platform
* multi-page crawl
* collating userbase datasets
* collating relevant collection sessions for reports
* parsing and report analysis
* interactive mining
* event contexts & interactive anaylsis
