# HelloWordRabbitMQ
Hello Word! RabbitMQ Java

Putting it all together

* You can compile both of these with just the RabbitMQ java client on the classpath:

 `$ javac -cp rabbitmq-client.jar Send.java Recv.java`

* To run them, you'll need rabbitmq-client.jar and its dependencies on the classpath. In a terminal, run the sender:


 `$ java -cp .:commons-io-1.2.jar:commons-cli-1.1.jar:rabbitmq-client.jar Send`

* then, run the receiver:


 `$ java -cp .:commons-io-1.2.jar:commons-cli-1.1.jar:rabbitmq-client.jar Recv`

