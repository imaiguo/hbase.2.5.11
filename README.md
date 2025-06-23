
# Apache HBase
- Apache HBase NoSQL columnar datastore

- https://hbase.apache.org is an open-source, distributed, versioned, column-oriented store modeled after Google' [Bigtable](https://research.google.com/archive/bigtable.html): A Distributed Storage System for Structured Data by Chang et al. Just as Bigtable leverages the distributed data storage provided by the Google File System, HBase provides Bigtable-like capabilities on top of [Apache Hadoop](https://hadoop.apache.org/).

- HBase是Hadoop的生态系统，是建立在Hadoop文件系统（HDFS）之上的分布式、面向列的数据库，通过利用Hadoop的文件系统提供容错能力。如果你需要进行实时读写或者随机访问大规模的数据集的时候，请考虑使用HBase！

- HBase作为Google Bigtable的开源实现，Google Bigtable利用GFS作为其文件存储系统类似，则HBase利用Hadoop HDFS作为其文件存储系统；Google通过运行MapReduce来处理Bigtable中的海量数据，同样，HBase利用Hadoop MapReduce来处理HBase中的海量数据；Google Bigtable利用Chubby作为协同服务，HBase利用Zookeeper作为对应。

-	Base 是一个高可靠、高性能、面向列、可伸缩的分布式数据库，主要用来存储非结构化和半结构化的松散数据，设计它的目的就是用于处理非常庞大的表——通过水平扩展的方式，用计算机集群就可以处理由超过 10 亿行数据和数百万列元素所组成的数据表。

- 参考 https://www.bookstack.cn/read/BigData-Notes/README.md
- hbase https://hbase.apache.org/book.html

## 配置文件参数说明
- 配置文件hbase-site.xml
- hbase.cluster.distributed
- 集群的模式，分布式还是单机模式，如果设置成false的话，HBase进程和Zookeeper进程在同一个JVM进程。