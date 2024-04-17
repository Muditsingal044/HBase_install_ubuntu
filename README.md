# Hbase_install_ubuntu
*************************************************
Hbase installation On Ubuntu
*************************************************

## 1. install ->

link - https://dlcdn.apache.org/hbase/3.0.0-beta-1          (. click -> hbase-3.0.0-beta-1-bin.tar.gz )


## 2. nano .bashrc -> 
export HBASE_HOME="/home/mudit/hbase/hbase-3.0.0-beta-1"
export PATH=$PATH:$HBASE_HOME/bin

## create two folder -> cmd
1. mkdir hbase-data
2. mkdir zookeeper
   
## 3. hbase-site.xml (edite) -> 

<configuration>
  <property>
    <name>hbase.rootdir</name>
    <value>file:///home/mudit/hbase-data</value>
  </property>
  <property>
    <name>hbase.zookeeper.property.dataDir</name>
    <value>/home/mudit/zookeeper</value>
  </property>
</configuration>


## 4. open cmd in hbase folder ->  cmd
bin/start-hbase.sh

## 5. Start hbase shell -> cmd
hbase shell

## 6. Stop hbase shell -> cmd
stop-hbase.sh
