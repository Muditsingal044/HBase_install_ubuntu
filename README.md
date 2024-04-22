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


## 4. open cmd in hbase folder ->  cmd
1. source ~/.bashrc
2. bin/start-hbase.sh

## 5. Start hbase shell -> cmd
1. hbase shell

## 6. Stop hbase shell -> cmd
1. stop-hbase.sh

## Again start hbase -> cmd
1. start-hbase.sh
2. hbase shell
