# HelloWordRabbitMQ
Hello Word! RabbitMQ Java

We'll write two programs in Java; a producer that sends a single message, and a consumer that receives messages and prints them out. We'll gloss over some of the detail in the Java API, concentrating on this very simple thing just to get started. It's a "Hello World" of messaging.

In the diagram below, "P" is our producer and "C" is our consumer. The box in the middle is a queue - a message buffer that RabbitMQ keeps on behalf of the consumer.

![Hello Word](https://www.rabbitmq.com/img/tutorials/python-one.png "Hello Word") 


Putting it all together

* You can compile both of these with just the RabbitMQ java client on the classpath:

 `$ javac -cp rabbitmq-client.jar Send.java Recv.java`

* To run them, you'll need rabbitmq-client.jar and its dependencies on the classpath. In a terminal, run the sender:


 `$ java -cp .:commons-io-1.2.jar:commons-cli-1.1.jar:rabbitmq-client.jar Send`

* then, run the receiver:


 `$ java -cp .:commons-io-1.2.jar:commons-cli-1.1.jar:rabbitmq-client.jar Recv`


