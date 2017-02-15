*CLUSTER:
- In a computer system, a cluster is a group of servers and other resources that act like a single system and enable high availability and, in some cases, load balancing and parallel processing.
- In personal computer storage technology, a cluster is the logical unit of file storage on a hard disk; it's managed by the computer's operating system. Any file stored on a hard disk takes up one or more clusters of storage.

*HADOOP CLUSTER:
- A Hadoop cluster is a special type of computational cluster designed specifically for storing and analyzing huge amounts of unstructured data in a distributed computing environment. 
- Such clusters run Hadoop's open source distributed processing software on low-cost commodity computers. 
- Hadoop clusters are known for boosting the speed of data analysis applications. They also are highly scalable: If a cluster's processing power is overwhelmed by growing volumes of data, additional cluster nodes can be added to increase throughput. Hadoop clusters also are highly resistant to failure because each piece of data is copied onto other cluster nodes, which ensures that the data is not lost if one node fails.


*RACK:

- For small clusters in which all servers are connected by a single switch, there are only two levels of locality: “on-machine” and “off-machine.” When loading data from a DataNode’s local drive into HDFS, the NameNode will schedule one copy to go into the local DataNode, and will pick two other machines at random from the cluster.

- For larger Hadoop installations which span multiple racks, it is important to ensure that replicas of data exist on multiple racks. This way, the loss of a switch does not render portions of the data unavailable due to all replicas being underneath it.

- HDFS can be made rack-aware by the use of a script which allows the master node to map the network topology of the cluster.

*RACK ARRANGEMENT IN HADOOP CLUSTER:

- Hadoop clusters are often referred to as "shared nothing" systems because the only thing that is shared between nodes is the network that connects them. 

- Large Hadoop Clusters are arranged in several racks. Network traffic between different nodes in the same rack is much more desirable than network traffic across the racks.
(REFER THE IMG. ATTACHED.)
