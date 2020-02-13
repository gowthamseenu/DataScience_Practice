Big Data Overview:
- A local proces will use the computation resorces of a single machine
- A distributed process has access to the computational resources across a number of 
  machines connected through a network
- After a certain point, it is easier to scale out to many lower CPU machines, than to
  try to scale up to a single machine with high a CPU.
- Distributed machines also have the advantage of easily scaling, you can just add
  more machines
- They also include fault tolerance, if one machine fails, the whole network can still
  go on.
- Let's discuss the typical format of a distributed architecture that uses Hadoop

Hadoop:
- Hadoop is a way to distribute very large files across multiple machines.
- It uses the Hadoop Distributed File System(HDFS)
- HDFS allows a user to work with large data sets.
- HDFS also duplicates blocks of data for fault tolerance
- It also then uses MapReduce
- MapReduce allows computations on that data
- HDFS will use blocks of data, with a size of 128MB by default
- Each of these blocks is replicated 3 times
- The blocks are distributed in a way to support fault tolerance
- Smaller blocks provide more parallelization during processing
- Multiple copies of a block prevent loss of data due to a failure of a node

MapReduce:
- MapReduce is a way of splitting a computation task to a distribued set of files
  (such as HDFS)
- It consists of a job Tracker and multiple Task Trackers
- The Job Tracker sends code to run on the Task Trackers
- The Task trackers allocate CPU and memory for the tasks and monitor the tasks on the
  worker nodes
  
Spark Overview:
- 
  




   