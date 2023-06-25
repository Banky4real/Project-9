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

## Connecting Jenkins to Github to retrieve source Codes using Webhooks

![successfully-enabled-webhooks](./Images/webhook-successfully-enabled-in-github-repository.png)

### First Successful Jenkins Build
![First-Jenkins-Build](./Images/Build-successful.png)

### Console output for first build
![Console-output](./Images/Console-output.png)

### Post Build Action Configuration
![New-Build-Triggered-after-postBuild-Action-configuration](./Images/new-build-triggered-after-changes-on-github-project.png)

### Location of artifacts on Jenkins Server
`ls /var/lib/jenkins/jobs/Project9/builds/2/archive/`
![Artifacts-Location-on-Jenkins-server](./Images/Location-of-artifacts-on-jenkins-server.png)

## Configuring jenkins to copy files to NFS Server Via SSH

### Publish over SSH plugin Installation

![publish-over-ssh-plugin-installation](./Images/publish-over-ssh-installed.png)

### Configuring projects to copy artifacts over to NFS

### Jenkins configured to send all files produced by build to mnt/apps

![copying-artifacts-over-to-NFS](./Images/project-to-copy-artifacts-from-NFS-returned-success.png)

### Console output after changes has been made to read-me

![Console-output-after-changes-have-been-made-to-readme](./Images/new-job-triggered-by-webhook-after-changes-made-to-readme.png)

### Making sure files are updated on NFS Server Successfully

![files-updated-on-NFS-server-successfully](./Images/files-updated-on-NFSSERVER-successfully.png)