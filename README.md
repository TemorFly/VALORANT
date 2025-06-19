Имя устройства       	IP-адрес            Направление            Шлюз по умолчанию
ISP (DHCP)		                              Internet	
ISP (HQ-RTR)	      172.16.4.1/28	           HQ-RTR	
ISP (BR-RTR)	      172.16.5.1/28	           BR-RTR	
HQ-RTR (ISP)      	172.16.4.2/28	            ISP	                  172.16.4.1
HQ-RTR (VLAN100)	 192.168.100.1/26	         HQ-SRV	
HQ-RTR (VLAN200)	 192.168.200.1/28	         HQ-CLI	
HQ-RTR (VLAN999)	 192.168.99.1/29		
HQ-SRV (VLAN100)	 192.168.100.2/26	         HQ-RTR	               192.168.100.1
HQ-SRV (VLAN999)	192.168.99.2/29		
HQ-CLI (VLAN200)	192.168.200.3/28	         HQ-RTR	               192.168.200.1
BR-RTR (ISP)	    172.16.5.2/28	              ISP	                  172.16.5.1
BR-RTR (BR-SRV)	    10.1.1.1/27	             BR-SRV	
BR-SRV	            10.1.1.2/27	             BR-RTR	                 10.1.1.1
HQ-RTR (tun1)    	172.16.100.1/28	   Туннель в сторону BR-RTR	
BR-RTR (tun1)	    172.16.100.2/28	   Туннель в сторону HQ-RTR	



UID для sshuser на HQ-SRV и BR-SRV 1010
Порт 2024
