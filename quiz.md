## Long Quiz in Advanced Systems Integration & Architecture
1. Define Service Oriented Architecture (SOA).
-It is a comprehensive strategy for software development across an entire enterprise, leveraging reusable software components known as services. These services consist of the necessary code and data integrations essential for performing specific business functions.

2. List and discuss the characteristics of SOA.
• Standardized Service Contracts: Services adhere to a service description. Services use service contracts to:
o Express their purpose
o Express their capabilities

• Loose Coupling: Services minimize dependencies on each other and create specific types of relationships within and outside of service boundaries with a constant emphasis on reducing dependencies between service contract, service implementation, and service consumers.

• Abstraction - Services hide the logic they encapsulate from the outside world.
o Avoids the proliferation of unnecessary service information, metadata, or data
o Hides as much of the underlying details of a service as possible
o Enables and preserves the loosely-coupled relationships.
o Plays a significant role in the positioning and design of service compositions

• Service Reusability: Logic is divided into services with the intent of maximizing reuse.

• Autonomy - Services should have control over the logic they encapsulate.
o Represents the ability of a service to carry out its logic independently of outside influences
o To achieve this, services must be more isolated
▪ Increased reliability
▪ Behavioral predictability

• Statelessness - Ideally, services should be stateless.
o Incorporate state management deferral extensions within a service design goal.
o Increase service scalability.
o Support the design of agnostic logic and improve service reuse.

• Discoverability - Services can be discovered (usually in a service registry).
o Service contracts contain appropriate metadata for discovery which also communicates purpose and capabilities to humans.
o Store metadata in a service registry or profile documents.

• Composability - Services break big problems into little problems. This is elated to the Reusability principle.
o Service execution should efficient in that individual processing should be highly tuned.
o Flexible service contracts to allow different types of data exchange requirements for similar functions.

• Interoperability
o Services should use standards that allow diverse subscribers to use the service.
o This is considered so obvious these days that it is often dropped as a principle.

3. Define Microservices.
-Microservices architectures consist of components that are loosely connected, reusable, and designed for specific purposes.

4. List and discuss the benefits of using Microservices.
-Microservices represent a genuine cloud-native architectural strategy. Their adoption facilitates easier code updates, the utilization of diverse stacks for individual components, and independent scaling of components, thereby minimizing waste and costs associated with scaling entire applications due to increased load on a single feature.

-Microservices, or microservices architecture, adheres to a cloud-native approach where a single application is constructed from numerous smaller components or services that are loosely connected and independently deployable.

-While the discourse around microservices often revolves around their architectural definitions and characteristics, their practical value becomes more apparent through straightforward business and organizational advantages, such as the ease of code updates and the ability for teams to employ different stacks for various components.

-Understanding microservices can also be approached by considering what they are not.

5. List and discuss the similarities and differences of SOA and Microservices.
-SOA aimed to establish a standardized communication and integration method across all services throughout an entire enterprise. Microservices architecture is tailored to a specific application. The key difference between the two lies in their scope: SOA has an enterprise-wide scope, whereas microservices architecture is focused on the scope of a particular application.

6. Define Web Services.
-A web service comprises open protocols and standards employed to exchange data between applications or systems.

7. List and discuss the benefits of using Web Services.
• Network Function Exposure
-A web service, a unit of managed code, can be activated remotely through HTTP, enabling the exposure of existing code functionality. Once exposed, other applications can utilize this program functionality.

• Interoperability
-Web services facilitate communication and data sharing between diverse applications, allowing platforms like VB or .NET to interact with Java web services and vice versa, ensuring technology independence.

• Standardized Communication
-Utilizing industry-standard protocols across layers, web services provide numerous advantages such as increased choices, cost reduction, and enhanced quality within the protocol stack.

• Cost-Effective Communication
-Web services implement SOAP over HTTP, enabling economical utilization of existing internet infrastructure. This proves more cost-effective than proprietary solutions like EDI/B2B, with flexibility for alternative transport mechanisms like FTP.

8. List and discuss the characteristics of Web Services.
• XML-Based
-Web services utilize XML for data representation and transportation, freeing them from networking, operating system, or platform constraints. This XML foundation ensures high interoperability at the core level of web services.

• Loosely Coupled
-Consumers of web services remain independent, allowing the web service interface to evolve without impacting the client's ability to interact. This contrasts with tightly coupled systems where changes in one interface necessitate updates in the other.

• Coarse-Grained
-Web services promote a coarse-grained approach, aligning with the need for business logic at a corporate level. Unlike individual methods in object-oriented technologies, web services enable the definition of services that access the appropriate amount of business logic.

• Synchronous or Asynchronous
-Web services offer flexibility in synchronicity, allowing clients to choose between synchronous and asynchronous operations. Synchronous invocations involve blocking until the service completes, while asynchronous operations enable clients to perform other functions and retrieve results later, supporting loosely coupled systems.

• Supports Remote Procedure Calls (RPCs)
-Clients can invoke procedures, functions, and methods on remote objects using an XML-based protocol. Web services expose input and output parameters, ensuring compatibility with RPCs.

• Supports Document Exchange
-XML's generic representation facilitates the transparent exchange of documents in web services, accommodating anything from simple addresses to complex documents like books or Requests for Quotation (RFQs). This capability enhances business integration.

9. List and discuss the distinct roles in Web Services Architecture.
Provider - This entity develops and offers a web service for use by client applications.
Requestor - The client application, written in languages like .Net or Java, seeks specific functionality through a web service.
Broker - The application providing access to UDDI, enabling client applications to discover web services.
Publish - The provider notifies the broker (service registry) of the web service's existence, making it accessible to clients.
Find - The requestor consults the broker to locate a published web service.
Bind - Armed with information from the broker, the requestor can invoke or bind to the web service.

10. List and discuss the Web Services Components.

SOAP is an XML-based communication protocol enabling information exchange across diverse operating systems. It provides a platform and language-independent solution by defining the encoding of HTTP headers and XML files for seamless communication, including compatibility with server firewalls.

WSDL, or Web Services Description Language, is an XML-based language describing web services and their access methods. Playing a vital role in UDDI, WSDL assists businesses in listing services on the Internet, facilitating navigation for individuals and businesses to access these services.

UDDI, or Universal Description, Discovery, and Integration, is an XML-based standard for describing, publishing, and discovering web services. Operating as an open, platform-independent framework, UDDI is one of the foundational standards of web services, along with SOAP and WSDL. It uses WSDL to define interfaces and serves as a specification for a distributed registry of web services.