# flume-playground
repo for a data streaming bootcamp 

#Plan for bootbacamp:
flume -> kafka -> spark streaming
#Command syntex to start the agent:
bin/flume-ng agent -n $agent_name -f conf/flume-conf.properties.template
step 1: create the config file
step 2: start the agent
flume-ng agent --name first-agent --conf-file first-agent.conf


step 3: send messages to post number given in conf-file
telnet <hostname> <port-number>
telnet flumehost.beercafeguy.com 44444

flume-ng agent --name log-agent --conf-file exec-memory-hdfs.conf