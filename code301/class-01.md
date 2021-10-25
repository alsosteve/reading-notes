# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 301

# Read: 01 - Introduction to React and Components

## Reading

### [Component Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)
**_Component Based Architecture_** breaks down how a page is designed into functional or logical components that represent communication interfaces containing methods, events, and properties. It divides problems into sub-problems. The primary objective is component reusability. 
Advantages are as follows:
* Reduced time time and cost by reusing existing components
* Increase in reliability with reused components

A **_Component_** is a software object that is modular, portable, replaceable, and reusable. It’s interface is defined by recommended behavior. It can work with other components.
It can be viewed in 3 ways:
1. Object-oriented - This viewing method shows components as one or more cooperating classes. 
2. Conventional - This shows functional elements or a program model.
3. Process-related -  builds from existing components in a library.

The characteristics are:
* reusability
* replacability
* not context specific
* extensible
* encapsulated
* independent

Advantages include: 
> points provided by tutorialpoints.com

Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance.

Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

Modification of technical complexity − A component modifies the complexity through the use of a component container and its services.

Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system.

Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

### [What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)
1. “Props” is short for properties.
2. Props are used as read only data. It is not to be changed by child components.
3. The flow of props is unidirectional. It flows one way, from parent to child.