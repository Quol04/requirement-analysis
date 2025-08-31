# Requirement Analysis in Software Development.
Requirement analysis is the process of gathering, documenting, and validating the needs and expectations of stakeholders for a software project.  

The purpose of this repository is to:  
- Provide structured notes and resources on requirement analysis.  
- Demonstrate how requirement analysis fits into the **Software Development Life Cycle (SDLC)**.  
- Share examples, templates, and best practices for documenting requirements.  

---

## 1. What is Requirement Analysis?  

Requirement Analysis is a critical phase of the **Software Development Life Cycle (SDLC)** where the project team identifies, gathers, and defines the functional and non-functional requirements of a system. It ensures that the final product aligns with business objectives and user needs.  

### Key Aspects of Requirement Analysis  
1. **Gathering Requirements**  
   - Collecting information from stakeholders through interviews, surveys, observations, and document analysis.  
2. **Documenting Requirements**  
   - Creating clear and structured requirement specifications such as Software Requirement Specifications (SRS).  
3. **Validating Requirements**  
   - Ensuring requirements are complete, consistent, feasible, and aligned with stakeholder expectations.  
4. **Managing Requirements**  
   - Handling changes effectively throughout the project to maintain project scope and quality.  

### Importance in the SDLC  
- **Foundation for Design**: Provides the blueprint for system architecture and design.  
- **Reduces Errors**: Catching unclear or conflicting requirements early minimizes costly rework later in development.  
- **Improves Communication**: Acts as a common reference point between stakeholders, designers, and developers.  
- **Ensures User Satisfaction**: By focusing on user needs, requirement analysis increases the likelihood of building a product that meets expectations.  

---

## 2. Why is Requirement Analysis Important?  

Requirement Analysis is vital to the success of any software project. Its importance can be highlighted in the following ways:  

1. **Prevents Scope Creep**  
   - Clearly defined requirements help establish the boundaries of a project. This reduces the chances of unexpected features being added later, which often cause delays and budget overruns.  

2. **Improves Project Planning and Estimation**  
   - Accurate requirements allow project managers to better estimate resources, costs, and timelines. This ensures that the development process is realistic and manageable.  

3. **Enhances Quality of the Final Product**  
   - By understanding both functional and non-functional needs early on, the development team can design and build software that meets user expectations, ensuring higher satisfaction and adoption rates.  

4. **Facilitates Better Communication**  
   - Requirement documents serve as a reference point for all stakeholders, ensuring everyone has a shared understanding of the system’s goals and features.  

5. **Reduces Risk and Rework**  
   - Identifying ambiguities, inconsistencies, or missing requirements at the beginning helps avoid costly errors later in the development lifecycle.  

In summary, requirement analysis lays the foundation for successful project execution, making it one of the most crucial activities in the SDLC.  

---

## 3. Key Activities in Requirement Analysis  

Requirement Analysis involves several structured activities that ensure stakeholder needs are properly captured, refined, and validated. The five key activities are:  

- **Requirement Gathering**  
  - Collecting raw requirements from stakeholders, clients, end-users, or existing documentation.  
  - Techniques include questionnaires, interviews, and reviewing business processes.  

- **Requirement Elicitation**  
  - Engaging with stakeholders to draw out hidden or implicit needs.  
  - Methods include workshops, brainstorming sessions, use case discussions, and prototyping.  

- **Requirement Documentation**  
  - Recording requirements clearly and systematically in formats such as Software Requirement Specifications (SRS).  
  - Helps create a reference for developers, testers, and stakeholders throughout the project.  

- **Requirement Analysis and Modeling**  
  - Examining gathered requirements to identify conflicts, redundancies, or feasibility concerns.  
  - Modeling techniques such as UML diagrams, flowcharts, or use case diagrams are often used to represent requirements visually.  

- **Requirement Validation**  
  - Ensuring requirements are correct, complete, and aligned with stakeholder needs.  
  - Involves stakeholder reviews, walkthroughs, and prototyping to confirm accuracy before design begins.  

---

## 4. Types of Requirements.

### Functional Requirements  

Functional requirements specify what the system must do — i.e., the features and capabilities the software must provide.

**Examples for a Booking Management Project:**
- **Search for hotels**: The system must allow users to search for hotels by city or geographical location.  
  *(Derived from the case study’s customer-side functional flows.)* :contentReference[oaicite:0]{index=0}  
- **View hotel details**: It must display room types, availability, pricing, and other relevant information for each hotel. :contentReference[oaicite:1]{index=1}  
- **Create a reservation (booking)**: The system must enable users to make hotel bookings/reservations. :contentReference[oaicite:2]{index=2}  
- **Cancel a reservation**: Users should have the ability to cancel their bookings as needed. :contentReference[oaicite:3]{index=3}  
- **Hotel management operations** (from the hotel manager’s perspective): These include the ability to onboard new hotels, update hotel details, upload images, and manage metadata. :contentReference[oaicite:4]{index=4}  

---

### Non-functional Requirements  
Non-functional requirements describe how the system performs — its quality attributes, constraints, and overall behavior under different conditions.

**Examples for a Booking Management Project:**
- **Consistency**: Once a booking is confirmed and paid for, the system must reflect that status immediately and consistently across all user views. :contentReference[oaicite:5]{index=5}  
- **Scalability and performance under load**: The system must handle a large number of read requests (e.g., hotel searches and viewing details), especially during peak traffic periods, without performance degradation. :contentReference[oaicite:6]{index=6}  
- **Reliability and availability**: The system should maintain high uptime, ensuring users can search and book hotels without interruptions — even during high-traffic events. (Also implied by the need to scale and manage heavy load.) :contentReference[oaicite:7]{index=7}   

---

## 5. Use Case Diagrams

### What is a Use Case Diagram?

A **Use Case Diagram** is a visual representation of how different users (actors) interact with a system. It shows the relationships between users and the major functions (use cases) the system provides.  

**Benefits of Use Case Diagrams:**
- Help stakeholders understand how the system will be used.
- Provide a clear overview of system functionality.
- Identify interactions between different actors and the system.
- Serve as a foundation for writing detailed use case descriptions and requirements.

---

### Use Case Diagram for Hotel Booking System

The main actors in the system include:
- **Customer** – searches, books, and cancels reservations.  
- **Hotel Manager** – manages hotel details, availability, and room information.  
- **Payment Gateway** – processes customer payments.  
- **System Admin** – oversees system health, user accounts, and security.  

**Primary Use Cases:**
- Search hotels  
- View hotel details  
- Make a reservation  
- Cancel reservation  
- Manage hotel information  
- Process payments  


![Hotel Booking Use Case Diagram](alx-booking-uc.png)

---

## 6. Acceptance Criteria
 
### Importance of Acceptance Criteria

Acceptance Criteria are specific, predefined conditions that a software product or feature must meet to be accepted by stakeholders, clients, or end-users. They serve as a **bridge between requirements and testing** by ensuring that everyone involved (developers, testers, product owners, and stakeholders) shares a clear understanding of what “done” means.  

**Benefits of Acceptance Criteria:**  
- Provide measurable standards to verify feature completion.  
- Reduce ambiguity in requirements.  
- Guide development and testing processes.  
- Ensure the delivered product meets business and user needs.  

---

### Example: Checkout Feature in the Booking Management System  

**Feature:** Checkout Process  

**Acceptance Criteria:**  
- The user must be able to view a summary of their booking (hotel name, room type, dates, price).  
- The system must provide at least two payment options (e.g., credit card, PayPal).  
- Payment details must be validated before processing.  
- Upon successful payment, a booking confirmation page must be displayed.  
- A confirmation email must be sent to the user within 5 minutes of successful checkout.  
- If payment fails, the user should be notified with an appropriate error message and allowed to retry.  


