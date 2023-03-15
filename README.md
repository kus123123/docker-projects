# docker-projects
This repo consist of various docker projects that i am trying
this is one is connection of mongodb-express to mongo db 
via docker compose
the issue .
I was facing during this project was how to open ports , listen ports and kill ports
the major commands in use are
port mapping -port you want to expose :application you are running
you can use the same application by changing the default ports .kindly make sure the port you expose is free or it will give an error that port is already in use.
to check which port are already in use is 
"sudo lsof -i -P -n | grep LISTEN "
to open ports we need to use command 
fuser -k 27017/TCP
or you can simply restart the pc (this worked for me simple )
i used docker desktop to view the containers process
