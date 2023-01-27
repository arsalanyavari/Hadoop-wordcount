# Hadoop-wordcount
Implementing word count using Hadoop map reduce (related to cloud computing course)

## Setup the project
First of all run ```cat mapper.py reducer.py > main.py```

Then create a file as input of this map reduxce program (name: tmpFile.txt); 

At the end run below command on your master node of cluster.

```bash
hadoop jar /usr/local/hadoop/share/hadoop/tools/lib/hadoop-streaming-3.3.4.jar -file main.py -mapper mapper.py -reducer reducer.py -input /tmpFile.txt -output /output
```
> __Warning__ : The version of hadoop-streaming might be different.

## Contributers
- [Amir Arsalan Yavari](https://github.com/arsalanyavari)
- [Mohammad Mahdi Barghi](https://github.com/mmahdibarghi)
