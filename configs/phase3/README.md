
configure terminal

interface Loopback0
 ip address 1.1.1.1 255.255.255.255
 no shutdown

interface GigabitEthernet0/1
 description Link-to-PE1
 ip address 10.1.2.1 255.255.255.252
 no shutdown

interface GigabitEthernet0/2
 description Link-to-PE2
 ip address 10.1.3.1 255.255.255.252
 no shutdown

end
write memory
