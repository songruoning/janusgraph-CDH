> 实际工作中遇到了JanusGraph与CDH的兼容问题，做了简单的尝试，能够把OLAP on SPARK任务跑起来了，希望对大家有帮助
> 
> In the previous work, I solved the compatibility issue between JanusGraph and CDH. I have made an uncomplicated operation to develop the OLAP task on the Spark Platform. I hope it can help your work.
> 
> - JanusGraph 0.2.3
> - CDH 5.7.6
> - hadoop-hdfs/yarn 2.6.0-cdh5.7.6
> - spark 1.6.0-cdh5.7.6-hadoop2.6.0-cdh5.7.6

实际项目中需要操作：

1. [关于需要新做的JanusGraph相关Jar/New jars related to JanusGraph](DIFF-cn.md)
2. [替换相应依赖Jar/Replace Jars](REMOVEJAR.md)
3. 将JanusGraph的lib分发至节点各个机器/Distribute the lib directory to other nodes。

`遇到问题可以提issue，共同来看`

[![JanusGraph logo](janusgraph.png)](http://janusgraph.org/)

JanusGraph is a highly scalable [graph database](http://en.wikipedia.org/wiki/Graph_database)
optimized for storing and querying large graphs with billions of vertices and edges
distributed across a multi-machine cluster. JanusGraph is a transactional database that
can support thousands of concurrent users, complex traversals, and analytic graph queries.

[![Build Status][travis-shield]][travis-link]
[![Maven][maven-shield]][maven-link]
[![Javadoc][javadoc-shield]][javadoc-link]
[![Codecov][codecov-shield]][codecov-link]
[![Coverity Scan][coverity-shield]][coverity-link]
[![Gitter][gitter-shield]][gitter-link]
[![Stack Overflow][stackoverflow-shield]][stackoverflow-link]

[travis-shield]: https://travis-ci.org/JanusGraph/janusgraph.svg?branch=master
[travis-link]: https://travis-ci.org/JanusGraph/janusgraph
[maven-shield]: https://img.shields.io/maven-central/v/org.janusgraph/janusgraph-core.svg
[maven-link]: https://search.maven.org/#search%7Cga%7C1%7Corg.janusgraph
[javadoc-shield]: https://javadoc.io/badge/org.janusgraph/janusgraph-core.svg?color=blue
[javadoc-link]: https://javadoc.io/doc/org.janusgraph/janusgraph-core
[codecov-shield]:https://codecov.io/gh/JanusGraph/janusgraph/branch/master/graph/badge.svg
[codecov-link]:https://codecov.io/gh/JanusGraph/janusgraph
[coverity-shield]: https://img.shields.io/coverity/scan/janusgraph-janusgraph.svg
[coverity-link]: https://scan.coverity.com/projects/janusgraph-janusgraph
[gitter-shield]: https://img.shields.io/gitter/room/janusgraph/janusgraph.svg
[gitter-link]: https://gitter.im/janusgraph/janusgraph
[stackoverflow-shield]: https://img.shields.io/badge/stackoverflow-janusgraph-blue.svg
[stackoverflow-link]: https://stackoverflow.com/questions/tagged/janusgraph

## Learn More

The [project homepage](http://janusgraph.org) contains more information on JanusGraph and
provides links to documentation, getting-started guides and release downloads.

## Community

* Chat: join us on [Gitter](https://gitter.im/JanusGraph/janusgraph)

* Stack Overflow: see the
  [`janusgraph`](https://stackoverflow.com/questions/tagged/janusgraph) tag

* Twitter: follow [@JanusGraph](https://twitter.com/JanusGraph) for news and
  updates

* Mailing lists:

  * **janusgraph-users (at) googlegroups.com**
    ([archives](https://groups.google.com/group/janusgraph-users))
    for questions about using JanusGraph, installation, configuration, integrations

    To join with a Google account, use the [web
    UI](https://groups.google.com/forum/#!forum/janusgraph-users/join); to
    subscribe/unsubscribe with an arbitrary email address, send an email to:

    * janusgraph-users+subscribe (at) googlegroups.com
    * janusgraph-users+unsubscribe (at) googlegroups.com

  * **janusgraph-dev (at) googlegroups.com**
    ([archives](https://groups.google.com/group/janusgraph-dev))
    for internal implementation of JanusGraph itself

    To join with a Google account, use the [web
    UI](https://groups.google.com/forum/#!forum/janusgraph-dev/join); to
    subscribe/unsubscribe with an arbitrary email address, send an email to:

    * janusgraph-dev+subscribe (at) googlegroups.com
    * janusgraph-dev+unsubscribe (at) googlegroups.com

## Contributing

Please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for more information, including
CLAs and best practices for working with GitHub.

## Users

The following users have deployed JanusGraph in production.

* [CELUM](https://www.celum.com/) - [use case and system architecture](https://www.celum.com/en/graph-driven-and-reactive-architecture)
* [FiNC](https://finc.com)
* [G DATA](https://gdatasoftware.com)
* [Seeq](https://seeq.com)
* [Sift Security](https://siftsecurity.com)
* [Uber](https://uber.com)

The following companies offer JanusGraph hosted as-a-service:

* [IBM](https://www.compose.com/databases/janusgraph)
