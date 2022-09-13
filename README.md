# Rocketloop Architecture Assignment - IoT Home Security Monitoring

Hi there 👋

Whether you have been sent this assignment in response to an interview with us or you have stumbled upon it by chance, we are excited you are here. Rocketloop is always looking for smart, passionate people that want to use their skills and talents to create awesome things, so if you are interested in taking on a new challenge, working with a world-class team of passionate and technology-loving people, we would love for you to take on this assignment.

## Objective

In this assignment, you are tasked with developing a scalable, maintainable, and secure software architecture for an IoT product.

### Prodcut Description

A home security monitoring system that uses different sensors and AI to detect break-ins and other emergencies in customer homes. There is a central dispatch center with employees that are responsible to monitor customer homes. When an emergency is detected in a home, the dispatcher should receive an alert in their monitoring dashboard in order to call emergency services (e.g. police or fire rescue). The sensors in each customer's home can include motion sensors, sound sensors, CO2 sensors, and door/window sensors. The individual sensors do not have an internet connection, so sensor data should be aggregated locally on a provided gateway/bridge (hardware similar to a raspberry pi) that then sends the sensor data to the cloud to be processed. We need to store all sensor data persistently for future use as training data for machine learning models. In addition, sensor data for each home must be analyzed in real-time by multiple ML models in order to detect emergencies. Each ML model takes a significant amount of time to be loaded into memory and might need specific hardware (GPUs). We are expecting roughly 10 sensors per home. Each sensor produces a reading every minute (roughly 10KB of data). The system should be able to scale to at least 1,000,000 homes.
Customers should have access to an app that shows them the status of their home, i.e. what sensors are installed, their status, and if the system is operational, from their mobile phone.

## Additional Considerations

When designing the software architecture, please also consider the following questions:

- How can we make sure that we do not lose sensor data in case of partial system outage?
- What steps can we take to make sure computing resources are used efficiently?
- How can we store the sensor data in a cost effective way?
- What could be strategies to reduce the amount of data that we need to ingest/process?
- How can we make sure that the software running on the local gateway is kept up to date?

## Deliverable

Your submission should consist of a high-level description of your proposed software architecture, including an introduction into the individual components that make up the architecture and a visual diagram of how the components interact. Additionaly, your submission should include a more detailed description of each component and the interactions each component has with the other components. Please also include any additional considerations and all documentation that would be necessary for the proposed software architecture to be communicated to a team of software engineers in order to be implemented.
