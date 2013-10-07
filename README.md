nagiosalert
===========

Nagios: (enable|disable) service notification on a host within a cluster.

# How to use
* download nagiosalert

```
$ git clone https://github.com/keisatou/nagiosalert.git

$ cd nagiosalert
```

* set location of nagios command file

see the following URL for the details on command file(External commands):  
http://nagios.sourceforge.net/docs/3_0/extcommands.html

```
$ vi nagiosalert.conf
ROOT='/usr/local/nagios'
# you can use placeholder <CLUSTER>
CNF_COMMANDFILE="${ROOT}/<CLUSTER>var/rw/nagios.cmd"
```

* execute nagiosalert

```
./nagiosalert enable host_name service_name cluster_name
```
