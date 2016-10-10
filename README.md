# spring-samples
Spring Framework Examples

This is a simple example using Spring Boot, Spring Integration, Spring JPA, and Spring MVC to create a Person object in a browser, and send that person over a message channel to a ReceivedPerson repository/database. You can that use methods to access that data in JSON format.

For example, run the SendPerson Application (runs on localhost:8080) and the ReceivedPerson applicaton (runs on localhost:8090), and go to localhost:8080 and create a person. You can than access all the data using an API which produces results in JSON.

You could go to localhost:8090 to see all the results, or to get a specific result go to localhost:8090/find/1. To delete a result you would go to localhost:8090/delete/1. The last variable represents the Id of the Person object.

The StreamListener is what actually listens for messages on an input channel, and then saves that object to a local embedded database in this example.

To run the application you must have Apache Kafka and Zookeeper installed. 

https://kafka.apache.org/quickstart - If you don't have Apache Kafka installed, go there and follow those instructions. After you download the code, you will only need to complete Step 2 which is starting zookeeper and Kafka in order to run this project.

Start Zookeeper, Start Kafka, and then run the SendPerson application and the ReceivedPerson application. After that you are ready to go.
