# Here are a few Linux commands all Linux admins should know and use.

### Prerequisites
1. Jenkins Master Running [Get help here](https://youtu.be/-0dkiteJEuE)
1. EC2 RHEL 7.x Instance - _for Slave Node_ [Get help here](https://www.youtube.com/watch?v=KDtS6BzJo3A)
   - With Internet Access
   - Security Group with Port `8080` open for internet
   - Java v1.8.x 

## Install Java
We will be using open java for our demo, Get latest version from http://openjdk.java.net/install/. Also configure the default `JAVA_HOME` path
```sh
yum install java-1.8*
#yum -y install java-1.8.0-openjdk
```
<role rolename="manager-gui"/>
        <role rolename="manager-script"/>
        <role rolename="manager-jxm"/>
        <role rolename="manager-status"/>
        <user username="admin" password="admin" role="manager-gui, manager-script, manager-jmx, manager-status"/>
        <user username="deployer" password="deployer" roles="manager-script"/>
        <user username="tomcat" password="s3cret" roles="manager-gui"/>


