```markdown
```mermaid
flowchart TB
    subgraph CobalToJava Architecture
        direction TB

        subgraph Presentation Layer
            direction TB
            ClientApp[Client Application]
            APIGateway[API Gateway]
        end

        subgraph Application Layer
            direction TB
            AuthService[OAuth Service]
            CobalToJavaService[CobalToJava Microservice]
            JavaGenService[Java Generation Service]
        end

        subgraph Integration Layer
            direction TB
            ExternalAPIs[External APIs Integration]
        end
        
        subgraph Data Layer
            direction TB
            CobolStorage[COBOL Files Storage]
            LogicDB[Business Logic Database]
            ValidationDB[Validation Rules Database]
        end
    end

    %% Connections
    ClientApp --> APIGateway
    APIGateway --> AuthService
    APIGateway --> CobalToJavaService
    AuthService <--> CobalToJavaService
    
    CobalToJavaService --> CobolStorage
    CobalToJavaService --> LogicDB
    CobalToJavaService --> ValidationDB
    CobalToJavaService --> ExternalAPIs

    CobalToJavaService --> JavaGenService

    %% Labels
    APIGateway:::label -->|Handles Requests| CobalToJavaService
    AuthService:::label -->|OAuth Integration| CobalToJavaService
    CobolStorage:::label -->|Stores Uploaded COBOL Files|
    LogicDB:::label -->|Stores Extracted Business Logic|
    ValidationDB:::label -->|Stores Validation Rules|
    ExternalAPIs:::label -->|Calls External APIs|
    JavaGenService:::label -->|Generates Java Microservices|

    %% Styles
    classDef label fill:#f9f,stroke:#333,stroke-width:2px;
    classDef external fill:#bbf,stroke:#333,stroke-width:2px;
    class ExternalAPIs external;
```
```