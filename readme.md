1.create database with name assignment( username password should be root for sql)
2. Unzip kafka zip file and paste the folder in C drive.
3. Open 2 Command prompt from kafka folder and run the below commands to start zookeeper and kafka server. 
Kafka Commands
Start Zookeeper  .\bin\windows\zookeeper-server-start.bat  .\config\zookeeper.properties

Start Kafka Server with bootstrap  .\bin\windows\kafka-server-start.bat  .\config\server.properties
Make Sure kafka is up and working.
make sure zookeeper and server are running.
4. Now run the java project and hit the URL
URL - http://localhost:8085/swagger-ui/index.html
5. When we update or perform any operation db will be updated.

GitHub - https://github.com/rsmaheshwari/motadata.git