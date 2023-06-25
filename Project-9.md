## **Documentation for Project 9**

### Installing JDK
`sudo apt update`
`sudo apt install default-jdk-headless`

![JDk-Installation](./Images/jdk-installed.png)

### Jenkins Installation
`sudo apt update`
`sudo apt-get install jenkins`

![Jenkins-Installation](./Images/Jenkins-Installation.png)

### Jenkins Up and running
`sudo systemctl status jenkins`
![Making-sure-Jenkins-is-up-and-running](./Images/jenkins-up-and-running.png)

## Jenkins Initial Setup

### Accessing jenkings from Browser
`http://<Jenkins-Server-Public-IP-Address-or-Public-DNS-Name>:8080`
![Accessing-Jenkins-from-Browser](./Images/Jenkins-accessed-from-Browser.png)

`sudo cat /var/lib/jenkins/secrets/initialAdminPassword`
![Retrieving-Jenkins-admin-default-password-from-Server](./Images/Jenkins-default-admin-password.png)

### Suggested Plugin Installation
![Installing-suggested-plugin](./Images/Installing-suggested-plugin.png)

### Jenkins Setup Complete
![Jenkins-setup-complete](./Images/jenkins-setup-complete.png)