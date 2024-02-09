# Apache-Zeppelin-Installation-Linux (Web based notebook that enables data-driven, interactive data analytics and collaborative documents with SQL, Scala, Python, R and more)
Apache Zeppelin Installation

First, JDK installation

  1) sudo mkdir -p /usr/lib/jvm
  
  
  2) Download JDK 
  https://download.oracle.com/java/21/latest/jdk-21_linux-x64_bin.tar.gz
  
  
  3) extract the tarball
  sudo tar zxvf jdk-21_linux-aarch64_bin.tar.gz -C /usr/lib/jvm
  
  
  4)  declare that java version available at:
  sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk-21.0.2/bin/java" 1
  
  
  5) Set the new JDK as the default
  
      sudo update-alternatives --set java /usr/lib/jvm/jdk-21.0.2/bin/java
  6) java -version

Second, Zeppelin-Installation:

1) Download Binary Package
https://dlcdn.apache.org/zeppelin/zeppelin-0.10.1/zeppelin-0.10.1-bin-all.tgz

2) Extract the file
sudo tar zxvf zeppelin-0.10.1-bin-all.tgz

3) Starting Apache Zeppelin
   
    cd zeppelin-0.10.1-bin-all/
   
    sudo bin/zeppelin-daemon.sh start

Change the configuration file to work with Zeppelin remotely and share your work with your colleagues. 

1) stop Zeppelin service 
bin/zeppelin-daemon.sh stop

2) go to   /zeppelin-0.10.1-bin-all/conf directory

3) sudo cp zeppelin-site.xml.template   zeppelin-site.xml

4) sudo nano zeppelin-site.xml

5) set "zeppelin.server.addr" to 0.0.0.0

Restart Zeppelin

1) cd zeppelin-0.10.1-bin-all
2) sudo bin/zeppelin-daemon.sh restart



