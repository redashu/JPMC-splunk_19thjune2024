## plan for the day 
<img src="plan.png">


### splunk architecture phase 1

<img src="phase1.png">

### understanding Splunk API and its connect port

```
/opt/splunk/bin/splunk show web-port
WARNING: Server Certificate Hostname Validation is disabled. Please see server.conf/[sslConfig]/cliVerifyServerName for details.
Web port: 8000
[root@jpmc-splunk-server ~]# 
[root@jpmc-splunk-server ~]# 
[root@jpmc-splunk-server ~]# /opt/splunk/bin/splunk show splunkd-port
WARNING: Server Certificate Hostname Validation is disabled. Please see server.conf/[sslConfig]/cliVerifyServerName for details.
Splunkd port: 8089
[root@jpmc-splunk-server ~]# 

```

### SPlunk for developers

<img src="splunkdev.png">


### setup SPLUNK_HOME env for config purpose 

### SPLUNK_HOME as Installlation directory 

```
SPLUNK_HOME=/opt/splunkforwarder/
PATH=$PATH:$SPLUNK_HOME/bin
export PATH
```

## making SPLUNK_HOME persistent after reboot or disconnect

```
echo  "SPLUNK_HOME=/opt/splunkforwarder/"  >>~/.bashrc
echo  "PATH=$PATH:$SPLUNK_HOME/bin"  >>~/.bashrc 
echo  "export PATH"  >>~/.bashrc 
```

