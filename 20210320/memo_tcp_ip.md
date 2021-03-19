

```bash
hirotaka@hirotaka-40:~$ sudo tcpdump -tn -i any icmp
[sudo] hirotaka のパスワード:         
tcpdump: verbose output suppressed, use -v or -vv for full protocol decode
listening on any, link-type LINUX_SLL (Linux cooked v1), capture size 262144 bytes
IP 192.168.0.11 > 8.8.8.8: ICMP echo request, id 5, seq 1, length 64
IP 8.8.8.8 > 192.168.0.11: ICMP echo reply, id 5, seq 1, length 64
IP 192.168.0.11 > 8.8.8.8: ICMP echo request, id 5, seq 2, length 64
IP 8.8.8.8 > 192.168.0.11: ICMP echo reply, id 5, seq 2, length 64
IP 192.168.0.11 > 8.8.8.8: ICMP echo request, id 5, seq 3, length 64
IP 8.8.8.8 > 192.168.0.11: ICMP echo reply, id 5, seq 3, length 64
^C
6 packets captured
6 packets received by filter
0 packets dropped by kernel
```

```bash
hirotaka@hirotaka-40:~$ traceroute -n 8.8.8.8
traceroute to 8.8.8.8 (8.8.8.8), 30 hops max, 60 byte packets
 1  192.168.0.1  3.398 ms  3.315 ms  3.293 ms
 2  210.173.146.32  7.842 ms  7.824 ms  7.873 ms
 3  210.173.145.69  7.788 ms  7.770 ms  7.751 ms
 4  210.173.150.97  7.732 ms 210.173.150.53  7.713 ms  7.665 ms
 5  103.246.232.96  12.061 ms  12.042 ms 210.171.224.96  13.670 ms
 6  108.170.242.161  11.038 ms  11.534 ms *
 7  108.170.235.45  14.165 ms 108.170.233.21  12.179 ms 8.8.8.8  15.272 ms
```


