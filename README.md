## MapReduce-Electricty-Problem-Example
MapReduce Electricty Problem Example  is one of the most common [as that of HELLO WORLD program] jar file example over online Tutorials.. 

Here I had Made a Small Change Since common example over internet is Troubleing me with some parseing errors:


### Reference
      +---------------------------------------------------------------+
      |  https://www.tutorialspoint.com/hadoop/hadoop_mapreduce.htm   |
      +---------------------------------------------------------------+


### OPERATIONS

DOWNLOAD FILES, CREATE A DIRECTORY AT HOME OF HADOOP USER, COPY FILES INTO IT, GIVE EXECUTABLE PERMISSIONS TO ALL USERS FOR THAT FOLDER


hadoop@ubuntu:~$ ```cd ~```

hadoop@ubuntu:~$ ```mkdir electricty_usage```

hadoop@ubuntu:~/electricty_usage$ ```cp <current path of downloaded files>  electricty_usage```

hadoop@ubuntu:~/electricty_usage$ ```sudo chmod -R 0777 .``` 

----------------------------- EITHER ------------------------------------------------------------

hadoop@ubuntu:~/electricty_usage$ ```$HADOOP_HOME/bin/hadoop fs -mkdir input0```

hadoop@ubuntu:~/electricty_usage$ ```$HADOOP_HOME/bin/hadoop fs -put sample_data.txt input0```

hadoop@ubuntu:~/electricty_usage$ ```$HADOOP_HOME/bin/hadoop fs -ls input0```   

hadoop@ubuntu:~/electricty_usage$ ```javac -classpath hadoop-core-1.2.1.jar -d units ProcessUnits.java``` 

hadoop@ubuntu:~/electricty_usage$ ```jar -cvf units.jar -C units/ .```  

hadoop@ubuntu:~/electricty_usage$ ```$HADOOP_HOME/bin/hadoop jar units.jar hadoop.ProcessUnits  inputtxt output01```

hadoop@ubuntu:~/electricty_usage$ ```$HADOOP_HOME/bin/hadoop fs -cat output01/*``` 
 

-----------------------------   OR   ------------------------------------------------------------

hadoop@ubuntu:~/electricty_usage$ ```source .commands``` 

hadoop@ubuntu:~/electricty_usage$ ```$_INPUT```   

hadoop@ubuntu:~/electricty_usage$ ```$_UPLOAD```  

hadoop@ubuntu:~/electricty_usage$ ```$_LIST```    

hadoop@ubuntu:~/electricty_usage$ ```$_COMPILE``` 

hadoop@ubuntu:~/electricty_usage$ ```$_BIND```    

hadoop@ubuntu:~/electricty_usage$ ```$_RUN```     

hadoop@ubuntu:~/electricty_usage$ ```$_OUT```    



----------------------------------------------------------------------------------------









### Commands

`$_INPUT`     =  Create input Folder inside HDFS 

`$_UPLOAD`    =  Upload Sample Data [To Be Processed] into HDFS

`$_LIST`      =  (OPTIONAL) LIST OUT HDFS



`$_COMPILE`   =  COMPILE JAVA CODE CODE

`$_BIND`      =  BIND JAVA BYTE CODE INTO .JAR FILE

`$_RUN`       =  RUN OUR JAR FILE USING MAPREDUCER

`$_OUT`       =  VIEW OUTPUT





### Sample Data
```
Year    Jan     Feb     Mar     Apr     May     Jun     Jul     Aug     Sept    Oct     Nov     Dec     Average

1979	23	23	24	43	24	25	26	26	26	26	25	26	25

1980	26	27	28	28	28	30	31	31	31	30	30	30	29

1981	31	32	32	32	33	34	35	36	36	34	34	34	34

.

.

.

1993	39	38	39	39	39	41	42	43	40	39	38	38	40

1994	38	39	39	39	39	41	41	41	00	40	39	39	45
```




### EXPECTED OUTPUT
```
1981	34

1982	32

1983	34

1984	40

1985	45

1986	34

1987	40

1988	45

1989	34

1990	40

1991	45

1992	34

1993	40

1994	45

```
