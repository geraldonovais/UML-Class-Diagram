# UML - Unified Modelling Language

Unified Modeling Language (UML) is a standardized modeling language used in software engineering to visualize, specify, construct, and document the structure and behavior of software systems. 

Developed by Grady Booch, Ivar Jacobson, and James Rumbaugh in the 1990s, UML provides a set of graphical notation techniques to create abstract models of software systems. These models help stakeholders understand complex systems, facilitate communication, and ensure that the software meets its requirements.

## ★ Purposes and Benefits

**Clarification and Communication:** UML diagrams serve as a common language between developers, analysts, and stakeholders. They clarify the design and requirements, making it easier to communicate complex ideas.

**Design and Planning:** UML aids in designing system architecture and planning the development process. It helps in creating blueprints for software that align with business goals.

**Documentation:** UML provides a structured way to document software designs and architecture, which is invaluable for maintenance, future development, and onboarding new team members.

**Analysis and Validation:** By visualizing the system, UML helps in analyzing requirements and validating that the design meets the intended goals and constraints.

## 🔗 Relationships in UML

UML defines various types of relationships to model different aspects of interactions and dependencies between classes and objects. Here’s an overview of some key relationships:

### 1. Association

Association represents a general relationship between two classes. It indicates that objects of one class are connected to objects of another class.

![Association](https://i.imgur.com/vzOjkpO.png)

Examples:

* Customer and Order: A Customer places multiple Orders, and each Order is associated with a Customer.
* Teacher and Student: A Teacher teaches multiple Students, and each Student is associated with a Teacher.
* Doctor and Patient: A Doctor can have multiple Patients, and each Patient can be associated with multiple Doctors for different health issues.

### 2. Aggregation

Aggregation is a type of association that represents a "whole-part" relationship where the part can exist independently of the whole. It’s a weaker relationship compared to composition.

![Aggregation](https://i.imgur.com/dUV4lyv.png)

Examples:

* Library and Book: A Library contains multiple Books, but each Book can exist outside the context of a particular Library.
* Engine and Car: A Car contains an Engine. An Engine can exist independently of a Car, even though it's typically used within one.
* Order and Items: An Order "has" Items. Items can exist independently of the Order (they might be canceled or modified).

### 3. Composition

Composition is a stronger form of aggregation where the lifetime of the part is dependent on the lifetime of the whole. If the whole is destroyed, the parts are also destroyed.

![Composition](https://i.imgur.com/OHVkbw3.png)

Examples:

* House and Room: A House is composed of several Rooms. If the House is demolished, the Rooms no longer exist.
* Chapter and Book: A Book is made up of several Chapters. If the Book is removed or destroyed, the Chapters are inherently lost as well.

### 4. Inheritance

Inheritance denotes a relationship where a class (subclass) inherits attributes and behaviors from another class (superclass). It models an "is-a" relationship.

![Inheritance](https://i.imgur.com/zLnzWJv.png)

Examples:

* Animal and Dog: Dog is a subclass of Animal, inheriting properties like eat() and sleep() from Animal.
* Vehicle and Car: Car is a subclass of Vehicle, inheriting characteristics like drive() and refuel() from Vehicle.
* Employee and Manager: Manager is a subclass of Employee, inheriting general employee properties but with additional managerial responsibilities.

### 5. Realization

Realization is a relationship between an interface and a class that implements that interface. It indicates that a class provides concrete behavior for the operations defined in an interface.

![Realization](https://i.imgur.com/9g6H3X0.png)

Examples:

* Drawable Interface and Circle Class: The Circle class might realize the Drawable interface, providing the implementation for the methods defined in the interface, such as draw().
* RemoteControl Interface and TV Class: The TV class might realize the RemoteControl interface, implementing methods to turn the TV on and off and change channels.
* Shape Interface and Classes Circle, Rectangle, Triangle: All implement the Shape interface, providing their specific implementations for calculating area and perimeter.

### 6. Dependency

Dependency indicates a relationship where one element (the client) depends on another element (the supplier) such that a change in the supplier may affect the client. This relationship is often used to show that one class uses another class or relies on it in some way.

![Dependency](https://i.imgur.com/kFL9vb6.png)

Examples:

* Class A and Class B: Class A might depend on Class B if Class A uses Class B’s methods or attributes.
* Class Logger and Class File: Logger might use File to write log messages to a file.
* Class DatabaseConnection and Class SqlConnection: DatabaseConnection might use SqlConnection to establish a connection to a database.
    
### 7. Association Class

Association Class is used to add attributes and operations to an association between classes. It represents a relationship that has its own properties and behavior.

![Association Class](https://i.imgur.com/0mwvapr.png)

Examples:

* Enrollment in a Course and Student: An Enrollment association class could link Course and Student and include attributes like enrollmentDate and methods for enrolling and dropping courses.
* Project Assignment between Employee and Project: The ProjectAssignment association class might include attributes such as assignmentDate and role, and operations for managing assignments.
* Contract between Supplier and Customer: A Contract association class could link Supplier and Customer, including details like contractTerms and startDate.
