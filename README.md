Switch>en
Switch#conf
Configuring from terminal, memory, or network [terminal]? 
Enter configuration commands, one per line.  End with CNTL/Z.

Switch(config)#vlan 2
Switch(config-vlan)#name v2
Switch(config-vlan)#exit
Switch(config)#vlan 3
Switch(config-vlan)#name v3
Switch(config-vlan)#exit
Switch(config)#vlan 4
Switch(config-vlan)#name v4
Switch(config-vlan)#exit

Switch(config)#interface fastEthernet 0/1
Switch(config-if)#switchport access vlan 2
Switch(config-if)#exit
Switch(config)#interface fastEthernet 0/2
Switch(config-if)#switchport access vlan 2
Switch(config-if)#exit

Switch(config)#interface fastEthernet 0/3
Switch(config-if)#switchport access vlan 3
Switch(config-if)#exit
Switch(config)#interface fastEthernet 0/4
Switch(config-if)#switchport access vlan 3
Switch(config-if)#exit

Switch(config)#interface fastEthernet 0/5
Switch(config-if)#switchport access vlan 4
Switch(config-if)#exit
Switch(config)#interface fastEthernet 0/6
Switch(config-if)#switchport access vlan 4
Switch(config-if)#exit
Switch(config)#
