# SF-Kafka-conn-ssl
First you need to create Truststores and Keystores. For that you need to run bash script file.
1. `cd secrets`
2. `bash ./create-certs.sh` OR `./create-certs.sh` "If that doesn't work you might wanna give it `CHMOD +x`
3. Then come back again `cd ..`
4. Run `docker-compose up` OR `sudo docker-compose up` (if permission is required)
5. Check for logs to see every service is running using and the commands are:
```docker-compose -f log <service name>, Forexample docker-compose -f log dev-kafka-1```
