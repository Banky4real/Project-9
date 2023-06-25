## **Documentation for Project 9**

### Installing JDK
`sudo apt update`
`sudo apt install default-jdk-headless`

![JDk-Installation](./Images/jdk-installed.png)

### TCP Port 80 Opened
![TCP-Port80](./Images/TCP-port-80-opened-in-security-group.png)

### Apache Load Balancer Installation and Enabling Module
`sudo apt update`
`sudo apt install apache2 -y`
`sudo apt-get install libxml2-dev`


`sudo a2enmod rewrite`
`sudo a2enmod proxy`
`sudo a2enmod proxy_balancer`
`sudo a2enmod proxy_http`
`sudo a2enmod headers`
`sudo a2enmod lbmethod_bytraffic`
![Enabling-Module-and-installing-apache-loadbalancer](./Images/Apache-load-balancer-and-module-enabling.png)

### Apache status verified as running
`sudo systemctl restart apache2`
`sudo systemctl status apache2`
![Apache-up-and-running](./Images/Apache-2-up-and-running.png)