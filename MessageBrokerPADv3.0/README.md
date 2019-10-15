# MessageBrokerPADv3.0

Steps for building and running the project (in IntelliJ IDEA):

1.Make sure you have Maven installed

2.Open IntelliJ IDEA, click Import Project, select the folder with the project downloaded from github and select Import Settings -> Maven

3.The project should build by itself in few seconds

4.Open src/main/java/labs/broker/QueueStorage.java 

5.Change the filePath on line 16 to an existing folder of your own

6.In the chosen folder create a file QueueStorage.json

7.Run the files in the following order: src/main/java/labs/broker/Main.java and src/main/java/labs/sender/Main.java

8.Send some messages (plain string) from the terminal opened by sender/Main.java

9.Run src/main/java/labs/receiver and you should be able to see received messages from sender one by one


Implemented functionalities:

1.Message Channel (Messaging Systems): possibility to send and receive messages using the message broker

2.Dead Letter Channel (Messaging Channels): the message are stored in an external JSON file so the messages may be received when the receiver comes online

3.Message Translator (Messaging Systems): the plain string is transformed to JSON for storing data

4.Content Enricher (Message Transformation): the time and data of creation is added to all mesages

5.Polling Consumer (Messaging Endpoints): the receiver can receive messages only one per 5 seconds
