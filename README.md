# Hbase_install_ubuntu
*************************************************
Hbase installation On Ubuntu
*************************************************

## 1. install ->

link - https://dlcdn.apache.org/hbase/3.0.0-beta-1          (. click -> hbase-3.0.0-beta-1-bin.tar.gz )


## 2. nano .bashrc -> 
1. export HBASE_HOME="/home/mudit/hbase/hbase-3.0.0-beta-1"                       
2. export PATH=$PATH:$HBASE_HOME/bin

## create two folder -> cmd
1. mkdir hbase_data
2. mkdir zookeeper
   
## 3. hbase-site.xml (edite) -> 

https://drive.google.com/file/d/1MljPp_in4pIkkcK2VwNo1n_qMcRoCehW/view?usp=sharing

## 4 cmd ->
1. hadoop fs -chmod g+w /tmp
2. hadoop fs -mkdir -p /user/hive/warehouse
3. hadoop fs -chmod g+w /user/hive/warehouse


## 5. open cmd in hbase folder ->  cmd
bin/start-hbase.sh

## 6. Start hbase shell -> cmd
hbase shell

## 7. Stop hbase shell -> cmd
stop-hbase.sh
