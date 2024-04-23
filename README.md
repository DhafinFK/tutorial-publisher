# Reflection Module 9: Publisher
## a. How many data your publlsher program will send to the message broker in one run?
In this tutorial the publisher sends five event so tht emessage broker during one run o fth program. these events are specifically instances of 'UserCreatedEventMessage' and are sent to the "user_created" and "user_createdx" queues. Four of the events are published to the "user_created" queue and one event ot the "user_craetedx" queue. Each 'publish event' call in the 'main' function sends one distinct event with unique 'user_id' and 'user_name' values.

## b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
The URL remains consistent across both the publisher and any potential subscriber programs, indicating they connect to the same AMQP server located at localhost on port 5672. This setup ensures that both the publisher and subscribers are interfacing with the same message broker, facilitating effective communication and message exchange. In this case, the URL specifies that the message broker is running on the same machine as the programs and uses the default port for AMQP. The "guest:guest" component signifies the username and password used to authenticate with the broker, which are often default credentials for local testing environments.

![alt text](images/image.png)