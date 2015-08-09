Get Java


Get MVN
https://maven.apache.org/
https://maven.apache.org/download.cgi
cd /tmp
wget http://apache.mirrors.tds.net/maven/maven-3/3.3.3/binaries/apache-maven-3.3.3-bin.tar.gz
tar xz apache-maven-3.3.3-bin.tar.gz
tar xf apache-maven-3.3.3-bin.tar
mv apache-maven-3.3.3/ /usr/local/maven
ln -s /usr/local/maven/bin/mvn /usr/bin/mvn




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


https://github.com/mirror/launch4j
https://github.com/lukaszlenart/launch4j-maven-plugin
