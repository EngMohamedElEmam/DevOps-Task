hazemsoliman9/dimension-website:latest


What i didnt do: change default port for apache => Ive exposed the port 10001 but I couldnt change the config files I tried downloading the files and editting them manualy then copy the files using the dockerfiler , i tried accessing the docker container using docker exec -it my_website /bin/bash and installing nano and changing the files then copied the files to my host laptop but again that failed for some reason. Would appreciate some guideness please. Thank you. 

For more context Ive changed the ports.conf file to listen to port 10001 then 000-default.conf <VirtualHost *:10001> however when i copy the files or run the container with mounting the files as a volume still the configs are the defaults

docker run -d -p 10001:10001 -p 8080:80 --name my_website hazemsoliman9/dimension-website
