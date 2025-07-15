These are kafka consumers which reads messages from producers.

Consumer1 and Consumer2 are Email and SMS microservices that take data from kafka topic and perform operations accordingly.

EmployeeCore is an EmployeeEvent class that contains all the Event data needed for serialization and deserialization. 

It has been kept separate so that multiple consumers can use it. Without this, we will need to create exact same event class in every consumer.
