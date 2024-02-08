# Apache-Zeppelin-Installation-Linux-
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
  5) java -version

  
  6)

Second, Zeppelin-Installation


