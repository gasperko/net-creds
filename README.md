Thoroughly sniff passwords and hashes from an interface or pcap file. Concatenates fragmented packets and does not rely on ports for service identification.

###Sniffs

* URLs visited
* POST loads sent
* HTTP form logins/passwords
* HTTP basic auth logins/passwords
* HTTP searches
* FTP logins/passwords
* IRC logins/passwords
* POP logins/passwords
* IMAP logins/passwords
* Telnet logins/passwords
* SMTP logins/passwords
* SNMP community string
* NTLMv1/v2 (HTTP, DCE-RPC, SMBv1/v2, LDAP, MSSQL, etc)
* Kerberos (Untested as I have no pcaps, just ripped straight from Pcredz)


###Examples

Auto-detect the interface to sniff

```sudo python net-creds.py```


Choose eth0 as the interface

```sudo python net-creds.py -i eth0```


Read from pcap

```sudo python net-creds.py -p pcapfile```


####Thanks
* Laurent Gaffie writer of PCredz
* psychomario writer of ntlmsspparser
