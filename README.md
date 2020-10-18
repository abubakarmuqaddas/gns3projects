GNS3 projects for Cisco certification practice

Useful commands:

Create empty volume for vManage:
  - qemu-img create -f qcow2 foobar.qcow2 100M

iptables rules for port forwarding:
  - iptables -A PREROUTING -t nat -i eth0 -p tcp --dport 80 -j DNAT --to 192.168.1.2:8080
  - iptables -A FORWARD -p tcp -d 192.168.1.2 --dport 8080 -j ACCEPT
