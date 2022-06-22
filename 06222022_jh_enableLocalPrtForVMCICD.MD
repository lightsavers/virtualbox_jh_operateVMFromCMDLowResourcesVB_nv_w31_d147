```
Author: lightsavers
Created: 06222022
```

# Enable Port Forwarding Between Host-Guest

 - Stop VM

 - Go to **Settings**
 
 - Go to **Network** 
 
 - Set **Attached to: NAT**
 
 - Expand **Advanced**
 
 - Click on **Port Forwarding**
 
 - Make entries:
 
```
 --------------------------------------------------------------------
| Name   | Protocol | Host IP   | Host Port | Guest IP  | Guest Port |
 --------------------------------------------------------------------
| Jenkins| TCP      | 127.0.0.1 | 8080      | 10.0.2.15 | 8080       |  
 --------------------------------------------------------------------
| ssh    | TCP      | 127.0.0.1 | 2222      | 10.0.2.15 | 22         | 
 --------------------------------------------------------------------
| web    | TCP      | 127.0.0.1 | 80        | 10.0.2.15 | 80         | 
---------------------------------------------------------------------
```

 - Start VM
 
 > Note: make sure VM has the ports above open.


