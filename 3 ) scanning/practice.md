# Scanning Tools : Hping3

Hping Command

1 ) ICMP Ping

CMD : hping3 -1 192.168.144.129

2 ) ACK scan on port 80

CMD : hping3 -A 192.168.144.129 -p 80

3 ) Scan UDP sacn on port 80

CMD : hping3 -2 192.168.144.129 -p 80

4 ) Collecting initial sequence number

CMD : hping3 192.168.144.129 -Q -p 139

5 ) SYN sacn on port 50-60

CMD : hping3 -8 50-60 -s 192.168.144.129 -v

6 ) FIN, PUSH and URG scan on port 80

CMD : hping3 -F -P -U 192.168.144.129 -p 80

7 ) Scan entire subnet for live host

CMD : hping3 -1 192.168.144.129 --rand-dest -I 80

8 ) Itercept all traffic containing HTTP signature

CMD : hping3 -9 HTTP -I eth0

9 ) SYN floding a victim

CMD : hping3 -s 192.168.144.129 -a 192.168.144.150 -p 22 --flood

