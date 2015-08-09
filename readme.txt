https://maven.apache.org/
https://maven.apache.org/download.cgi
cd /tmp
wget http://apache.mirrors.tds.net/maven/maven-3/3.3.3/binaries/apache-maven-3.3.3-bin.tar.gz
tar xz apache-maven-3.3.3-bin.tar.gz
tar xf apache-maven-3.3.3-bin.tar
mkdir /opt/maven
mv apache-maven-3.3.3/ /opt/maven
ln -s /opt/maven/bin/mvn /usr/bin/mvn
gedit /etc/profile.d/maven.sh
Add the following contents to /etc/profile.d/maven.sh :
    #!/bin/bash
    MAVEN_HOME=/opt/maven
    PATH=$MAVEN_HOME/bin:$PATH
    export PATH MAVEN_HOME
    export CLASSPATH=.

Save and close the file. Then: 
chmod +x /etc/profile.d/maven.sh
source /etc/profile.d/maven.sh
[for Centos7]


--building   
mvn install
mvn jar:jar

--start server (linux)
$./server1.sh
--start server (win32)
cmd>srvW32.cmd



--start client (linux)
$./cl1.sh
--start client (win32)
cmd>runner.cmd

