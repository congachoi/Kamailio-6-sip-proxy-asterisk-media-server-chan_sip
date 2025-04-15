TEST 1 server Kamailio standalone + multi server asterisk as Media server


# Rocky Linux 8
# Kamailio 6 - ip = 192.168.31.10
# MariaDB
# install rsyslog
# sip proxy(registrar + route load balance to Asteriks)
# kamctl add 1000 1234
# kamctl add 1001 1234
# kamctl dispatcher add 1 sip:192.168.31.17:5060 0 0 '' 'Media Gateway 1' 
# kamctl dispatcher add 1 sip:192.168.31.18:5060 0 0 '' 'Media Gateway 2'
# kamctl dispatcher show

# Asterisk 13 Chan_sip 192.168.31.17 & 192.168.31.18
