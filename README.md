# BlogPost_Microservices
## A brief note on microservices
A single microservice contains all the routing, middleware, business logic and database access to implement one feature of our app. All services are standalone services. We can write different services in different languages. For example, Comments services could have been built on ASP.NET while the post services could have been built on node.js
### Here in this project, we would be building a mini microservice app where a user can post something and then some different user can add comments on the post.
Comments and Post will be two different microservices. We would be communicating between these services through async solution using an event bus.
Although we can use readily available open sources like 

•	RabbitMQ

•	Kafka

•	NATS, etc 

### For event bus but we would be creating our own event bus using express and JavaScript a very simple one.
These microservices are completely built in **node.js and react.js**

**•	Post service running on port 4000**

**•	Comment service running on port 4001**

**•	Query Service on port 4002**

**•	Event Bus on port 4005**

**•	React app on port 3000.**
