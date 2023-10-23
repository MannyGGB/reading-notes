# Reading 01

(https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

- What is a “component”? "A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities." Components are deployed independently, and are reusable and replaceable.
- What are the characteristics of a component?

  - "Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

  - Replaceable − Components may be freely substituted with other similar components.

  - Not context specific − Components are designed to operate in different environments and contexts.

  - Extensible − A component can be extended from existing components to provide new behavior.

  - Encapsulated − A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

  - Independent − Components are designed to have minimal dependencies on other components."

- What are the advantages of using component-based architecture?

  - "Reduced time in market and the development cost by reusing existing components."
  - "Increased reliability with the reuse of the existing components."
  - "**Ease of deployment** − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
  - **Reduced cost** − The use of third-party components allows you to spread the cost of development and maintenance.
  - **Ease of development** − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
  - **Reusable** − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
  - **Modification of technical complexity** − A component modifies the complexity through the use of a component container and its services.
  - **Reliability** − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
  - **System maintenance and evolution** − Easy to change and update the implementation without affecting the rest of the system.
  - **Independent** − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development."

(https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)

- What is “props” short for? Properties. "Props are arguments passed into React components." — w3schools.com
- How are props used in React? Props are used to pass data from one component to another. This data is read-only; it should not be changed by the child.
- What is the flow of props? It flows in one direction, from parent to child.
