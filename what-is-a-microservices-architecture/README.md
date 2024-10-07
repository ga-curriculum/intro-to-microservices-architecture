<h1>
  <span class="headline">Intro to Microservices Architecture</span>
  <span class="subhead">What is a Microservices Architecture?</span>
</h1>

**Learning objective:** By the end of this lesson, learners will be able to explain the key characteristics of microservices architecture, identify its benefits and drawbacks, and describe how microservices operate independently while remaining loosely coupled in a distributed system.

![cinema microservices](./assets/cinema-microservices.png)

<!-- Quote -->

A microservice is a single self-contained unit which, together with many others, makes up a large application. By splitting your app into small units every part of it is independently deployable and scalable, can be written by different teams and in different programming languages and can be tested individually. — Max Stoiber

<!-- Quote -->

A microservice architecture means that your app is made up of lots of smaller, independent applications capable of running in their own memory space and scaling independently from each other across potentially many separate machines. — Eric Elliot

## What is a Microservices Architecture?

**[Adrian Cockroft](https://g.co/kgs/YQmtE9K)**, an engineer who oversaw Netflix transition from a monolithic to a microservices architecture defines it as a service‑oriented architecture composed of loosely coupled elements that have bounded contexts.

Loosely coupled means that you can update the services independently. Updating one service doesn’t require changing any other services. If you have a bunch of small, specialized services but still have to update them together, they’re not microservices because they’re not loosely coupled. One kind of coupling that people tend to overlook as they transition to a microservices architecture is database coupling, where all services talk to the same database and updating a service means changing the schema. You need to split the database up and denormalize it.

<br>

<div class="activity discussion">
  <h2 class="title">What are the benefits of microservices?</h2>
  <span class="minutes">10</span>
</div>

<br>

Let's discuss some of the benefits of using this style of architecture:

| **Benefits**                                    | **Details**                                                                 |
|---------------------------------------------|-----------------------------------------------------------------------------|
| **Faster application startup times**        | Microservices allow applications to start up more quickly since each service is smaller and starts independently. |
| **Quicker and more efficient deployments**  | Deployments are faster and more streamlined because individual services can be deployed separately without affecting the entire system. |
| **Independent service deployment**          | Each microservice can be deployed on its own, allowing for frequent updates and new versions without downtime for other services. |
| **Easier to scale and improve performance** | Microservices can be scaled individually, allowing teams to allocate more resources to specific services, leading to better overall performance. |
| **No long-term commitment to a technology stack** | Each new microservice can be built using different technologies, providing flexibility to choose the best stack for the task. |
| **More organized and focused services**     | Microservices are typically more organized, as each one focuses on a specific job, making the architecture easier to manage. |
| **Greater flexibility for reconfiguration** | Decoupled microservices can be reconfigured for different applications, such as serving both web clients and public APIs, without impacting the core system. |


<br>

<div class="activity discussion">
  <h2 class="title">What are the drawbacks of microservices?</h2>
  <span class="minutes">10</span>
</div>

<br>

Let's discuss some of the challenges that come with using a microservices architecture:

| **Challenges**                                    | **Details**                                                                 |
|---------------------------------------------|-----------------------------------------------------------------------------|
| **Developers must manage increased complexity** | Microservices add complexity, as developers must manage a distributed system with multiple services communicating across networks. |
| **Operational complexity in production**    | Managing and deploying a large number of services in production can be more complex, requiring sophisticated monitoring and orchestration tools. |
| **Unforeseen cross-cutting concerns**      | During implementation, teams may encounter issues like security, logging, or data consistency that weren’t anticipated during the design phase. |

<br>
