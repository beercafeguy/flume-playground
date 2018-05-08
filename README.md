# flume-playground
repo for a data streaming bootcamp 

### Plan for bootbacamp: <br>
flume -> kafka -> spark streaming <br>
#### Command syntex to start the agent: <br>
`bin/flume-ng agent -n $agent_name -f conf/flume-conf.properties.template`
<br>
#### step 1: create the config file<br>
#### step 2: start the agent<br>
`flume-ng agent --name first-agent --conf-file first-agent.conf`

#### step 3: send messages to post number given in conf-file
```
telnet <hostname> <port-number>
telnet flumehost.beercafeguy.com 44444

flume-ng agent --name log-agent --conf-file exec-memory-hdfs.conf

flume-ng agent \
--classpath "/user/beercafeguy/code/flume/lib/*" \
--name mp-agent \
--conf-file multiplexed_agent.conf


flume-ng agent \
--name fk-agent \
--conf-file flume_kafka_agent.conf