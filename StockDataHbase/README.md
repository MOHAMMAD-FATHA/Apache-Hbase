Hbase version : 1.4.6
Python version : 3.9.5

We will start with python program now(install happybase libarary by command pip3 install happybase), here we have python file stockdatahbase.py
After that start your hadoop and hbase i,e
$ start-all.sh
$ start-hbase.sh
$ jps
$ start-daemon.sh start thrift

Connect to the Hbase using happybase library

Create Hbase table using python happybase library

importing data using API URL into the Hbase table

Display the Hbase table using python happybase library

You can check the output at the terminal by running python program

You can check that at hbase table from the shell 
$ hbase shell
You will enter into the shell command

Now we can scan the table RealStockData in shell
hbase(main):007:0> scan ‘RealStockData’
