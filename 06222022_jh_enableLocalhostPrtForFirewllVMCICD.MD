```
Author: lightsavers
Created: 06222022
```

# Firewall Settings (Centos7 Guest)

Ports are closed by default. Therefore, one must open only the ports that apply. 

# Sample Scenario

1. Power on the VM locally or in your public cloud provider

2. Logging with your username with sudo powers

3. Starting opening ports as applicable to your project

4. For example, open port 80 TCP to allow HTTP users

```
sudo firewall-cmd --permanent --add-port=80/TCP  
```

5. For example, open port 443 TCP to allow HTTPS users

```
sudo firewall-cmd --permanent --add-port=443/TCP  
```

6. For example, open port 8080 TCP to allow applications like Jenkins

```
sudo firewall-cmd --permanent --add-port=8080/TCP  
```

7. For example, open port 22 TCP to allow SSH connections

```
sudo firewall-cmd --permanent --add-port=22/TCP  
```

8. List all the ports you have open

```
sudo firewall-cmd --list-ports  
```

9. List all services

```
sudo firewall-cmd --list-services  
```

10. Finally, reload firewall to commit the changes

```
sudo firewall-cmd --reload 
```

