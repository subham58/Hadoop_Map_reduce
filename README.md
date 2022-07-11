![SS4](https://user-images.githubusercontent.com/48358012/178337682-b9ca11b3-8828-4273-9693-06afd88a1bcd.PNG)
# Hadoop_Map_reduce
Basically It's a Hadoop Map reduce program word count program which mainly shows the count of each word in a text file.
Here it  shows  the implementation of Word Count java program in HDFS.
Below given is the commands to run the program in Windows.

1)Putting files in a directory created in hadoop:
--> hadoop fs -put C:/file1.txt /word_count
 --> hadoop fs -put C:/file2.txt /word_count

2)Checking what text is present in the files:
--> hadoop dfs -cat /word_count/file1.txt
 --> hadoop dfs -cat /word_count/file2.txt
   
3)Running the jar file:
 -->hadoop jar C:/hadoop-3.3.0/share/hadoop/mapreduce/hadoop-mapreduce-examples-3.3.0.jar wordcount /word_count /outputs

4)To see the occurence of each word:
hadoop fs -cat /outputs/*
