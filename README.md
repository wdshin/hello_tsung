# hello_tsung

## install tsung in Ubuntu 16.04

* git clone https://github.com/processone/tsung
* cd tsung
* ./configure
* make
* make install
* tsung -v 

## test example#1

* git clone https://github.com/wdshin/hello_tsung

* cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
( to allow localhost ssh without password prompt)
* ( if not exist, do "ssh-keygen -t rsa" )
* chmod og-wx ~/.ssh/authorized_keys
* run localhost with port 8080 and serving /hello
* tsung -f test1_locahlhost_hello.xml start
* cd ~/.tsung/log/
* ( change directory to latest log )
* /usr/lib/tsung/bin/tsung_stats.pl
* DISPLAY=:0.0 firefox report.html

## Read http://tsung.erlang-projects.org/user_manual/configuration.html

