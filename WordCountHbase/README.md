Hbase versio : 1.4.6
Python version : 3.9.5

Word Count program using happybase library in python:
First step is to we have to download the output of word count from HDFS to store that data in HBASE
$ hadoop fs -get /home/fatha/Documents/HBase/WordCountHbase /WordCountVideo/output/part-m-00000
After that we have to download happybase library to connect to hbase
$ pip3 install happybase
Now we will start with python program now, here we have python file WordCountHbase.py
After that start your hadoop and hbase i,e
$ start-all.sh
$ start-hbase.sh
$ jps
$ start-daemon.sh start thrift


Connect to the Hbase using happybase library(happybase.connection)

Create Hbase table using python happybase library

Importing word count data into the Hbase table

Display the Hbase table using python happybase library

You can check the output at the terminal

You can check that at hbase table from the shell 
$ hbase shell
You will enter into the shell command

Now we can scan the table WordCount1 in shell
$ scan ‘WordCount1’
