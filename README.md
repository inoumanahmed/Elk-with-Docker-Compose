Hello  i am setting up ELK Stack with Docker-Compose file and show the Logs of remote vm 

Diretory Setup: 
        => elk-stack 
               > docker-compose.yml
               > logstash.conf 
               > .env
        then create "esdata" directory for vloume mount inside the "elk-stack directory"

Follow these step: 
1: Create a directory for Elk-Stack to save these files in same directory
2: Copy these files from and "run docker-compose up -d" to create the container
3: After creating and running container then run kibana on localhost with port # i.e 192.168.1.79:5601        #change ip according to your setup 
4: Hope so all is running Well !!! 

Setup Remote VM (ip of my remote vm is 192.168.1.74)                                                          #change ip according to your setup 

1: Install Filebeat on remote vm 
2: Goto the /etc/filebeat/filebeat.yml                                             # you only configure Logstash Input & Logstash Output Configuration i also mention in file 
3: Edit filebeat.yml and configure it as you needed 
4: I am also uploading filebeat.yaml file. 
5: After make changes then restart filebeat services again
6: Open a Kibana Server it show you logs of your remote vm 
