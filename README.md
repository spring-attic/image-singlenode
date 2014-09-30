# Spring XD Single Node
This Docker image runs Spring XD in [single node](http://docs.spring.io/spring-xd/docs/1.0.0.BUILD-SNAPSHOT/reference/html/#_start_the_runtime_and_the_xd_shell) mode.
A single process is spawned that contains everything you need to get started:
 * A Spring XD Admin server exposes the REST API over http (port 9393, which is EXPOSEd via Docker)
 * A Spring XD container
 * An embedded ZooKeeper server
 * An embedded HSQLDB server for batch jobs.

That setup uses the 'local' MessageBus and Analytics will be stored _in memory_.