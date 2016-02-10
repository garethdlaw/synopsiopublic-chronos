##CHRONOS IMAGES

Enter all parameters as environment variables with leading CHRONOS_


docker run -d \
-e CHRONOS_HTTP_PORT=4400 \
-e CHRONOS_MASTER=zk://node-1:2181,node-2:2181,node-3:2181/mesos \
-e CHRONOS_ZK_HOSTS=node-1:2181,node-2:2181,node-3:2181 \
--name chronos --net host --restart always synopsiopublic/chronos:2.4.0-ubuntu-14.04
