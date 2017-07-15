


Nagios 

Nagios differentiates between two basic classes of checks: 
• Active checks: These are initiated by Nagios. Nagios can execute code in plugins regularly. The outcome of the code execution determines whether the check fails or not. Active checks are the most common and are useful and easy to set up with many types of services, such as HTTP, SSH, and databases. 
• Passive checks: These originate from a system other than Nagios, and the system notifies Nagios rather than Nagios polling it. These are useful in special situations, for instance, if the service being monitored is behind a firewall or if the service is asynchronous and it would be inefficient to monitor it with polling.


Ganglia
Ganglia is a graphing and monitoring solution for large clusters. It can aggregate information in convenient overview displays. The word "ganglia" is the plural form of ganglion, which is a nerve cell cluster in anatomy. The analogy implies that Ganglia can be the sensory nerve cell network  in your cluster. 


Graphite
While Munin is nice because it is robust and fairly easy to start using, the graphs it provides are only updated once in a while, normally every fifth minute. There is therefore a niche for a tool that does graphing that is closer to real time. Graphite is such a tool. 


Log handling Log handling is a very important concept, and we will explore some of the many options, such as the ELK (Elasticsearch, Logstash and Kibana) stack. Traditionally, logging just consisted of using simple print statements in code to trace events in the code. This is sometimes called printf-style debugging, because you use traces to see how your code behaves rather than using a regular debugger. 
