# WEB Application Development Prompt

## Application Type: Web Application
## Category: Full-Stack Development
## Template: spring.net

---

**IMPORTANT**: This is a comprehensive development prompt for building a web application. Follow ALL guidelines, standards, and precautions outlined below for optimal code quality, security, and maintainability.

## Project Description
cobol migration project to java

## 🎯 Project Overview

**Description**: cobol migration project to java

**Key Features to Implement**:


**Development Approach**: Follow the guidelines and standards outlined in this prompt to ensure high-quality, maintainable, and secure code.

## 📋 Project Reference Documents

> **Note for AI coding tools**: Read the full documents referenced below for complete context before implementing.

### Requirements Specification

# CobalToJava Project Requirements Document

## 1. Project Overview

The CobalToJava project aims to develop a system that facilitates the transformation of COBOL programs into Java microservices. The system should enable users to upload COBOL programs, automatically extract business logic, validations, and external API interactions from these programs, and subsequently generate new microservices using Java Spring Boot. The project also requires that these microservices be accessible via a micro
...

📄 **Full document**: @docs/requirements.md

---

### Technology Stack & Architecture

# Project: CobalToJava - Technology Recommendations

## 1. Frontend Technologies
For the front end, we need technologies that support modern web standards, are easy to maintain, and integrate well with microservices.

- **React.js**: This JavaScript library is widely used for building user interfaces, particularly single-page applications where you need a fast, responsive experience. It is highly compatible with RESTful APIs and can easily handle OAuth-based authentication flows.
  
...

📄 **Full document**: @docs/techstack.md

---

### Frontend Implementation Guide

# CobalToJava Frontend Implementation Guide

This guide provides a detailed blueprint for implementing the frontend of the CobalToJava project. It covers the component structure, state management, UI/UX guidelines, and code examples to help you effectively build and integrate the required features.

## 1. Component Structure

### Main Components

1. **FileUploadComponent**
   - **Purpose**: To upload COBOL programs.
   - **Features**: Drag-and-drop area, file validation, progress indicator.

...

📄 **Full document**: @docs/frontend.md

---

### Backend Implementation Guide

```markdown
# CobalToJava Backend Implementation Guide

**Version: 1.0**  
**Date: 2/6/2026**

## Table of Contents
1. [API Design](#api-design)
2. [Data Models](#data-models)
3. [Business Logic](#business-logic)
4. [Security](#security)
5. [Performance](#performance)
6. [Code Examples](#code-examples)

---

## API Design

### Endpoints

1. **Upload COBOL Program**
   - **Endpoint**: `/api/upload-cobol`
   - **Method**: POST
   - **Payload**: Multipart file upload
   - **Response**: 
...

📄 **Full document**: @docs/backend.md

---

### Application Flow & User Journeys

# CobalToJava System Flow Documentation

## 1. User Workflows

### Overview
Users will interact with the CobalToJava system through a web-based interface that communicates with backend microservices. The primary actions users can perform include uploading COBOL programs, reviewing extracted business logic, and generating Java microservices.

### User Journey

```mermaid
graph TD;
    A[Start] --> B[User logs in with OAuth]
    B --> C[Upload COBOL Program]
    C --> D[System Processes File]
...

📄 **Full document**: @docs/flow.md

---

### Project Status & Progress

# Project Status Tracking Template: CobalToJava

## 1. Implementation Phases

### Phase 1: Initial Setup
- Set up project repository and development environment
- Define and document architecture and design
- Integrate OAuth authentication

### Phase 2: COBOL Program Handling
- Develop functionality to upload COBOL programs
- Implement COBOL parser to extract business logic, validations, and external APIs

### Phase 3: Microservices Development
...

📄 **Full document**: @docs/status.md

---

### diagram_sequence

Certainly! Below is a Markdown file with Mermaid.js sequence diagrams illustrating key user flows for the "CobalToJava" project. Each sequence diagram captures a different aspect of the system, including authentication, data operations, and main features.

```markdown
# CobalToJava Sequence Diagrams

## 1. User Authentication Flow
```mermaid
sequenceDiagram
    actor User
    participant ClientApp
    participant AuthServer as OAuth Server
    
    User ->> ClientApp: Request Authentication
...

📄 **Full document**: @docs/diagram_sequence.md

---

### diagram_component

Here's a markdown file with a Mermaid.js flowchart representing a component diagram for the CobalToJava project. The diagram is organized into layers (Frontend, Backend, Data, External) with relationships and dependencies:

```markdown
```mermaid
flowchart TB
    %% Define subgraphs for each layer
    subgraph Frontend
        UI[User Interface]
    end

    subgraph Backend
        APIG[API Gateway]
        Auth[OAuth Service]
        COBOLUploader[COBOL Uploader Service]
...

📄 **Full document**: @docs/diagram_component.md

---

### diagram_architecture

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

...

📄 **Full document**: @docs/diagram_architecture.md

---

### Product Requirements Document (PRD)

# Product Requirements Document (PRD)

## 1. Introduction

Changed Again.The CobalToJava project aims to facilitate the modernization of legacy systems by providing a platform that can convert COBOL programs into Java-based microservices. This project will allow users to upload COBOL programs and automatically extract their business logic, validations, and external API calls. The extracted information will be used to generate new microservices built on the Java Spring Boot framework. The solutio
...

📄 **Full document**: @docs/prd.md

## 🏗️ Architecture Guidelines

**Pattern**:
- Full-stack monorepo or separate repos, API-first design approach, Shared type definitions, Microservices or monolithic architecture

**Description**:
- Application architecture pattern

**Structure**:
- **directories**: Full-stack monorepo or separate repos, API-first design approach, Shared type definitions, Microservices or monolithic architecture
- **files**: Client-server communication patterns, Database to API to frontend flow, Real-time updates (WebSockets, SSE), Caching strategies across layers
- **conventions**: File-based routing (Next.js style), API route organization, Protected routes and middleware, SEO-friendly routing

**Data Flow**:
- Client-server communication patterns, Database to API to frontend flow, Real-time updates (WebSockets, SSE), Caching strategies across layers

**State Management**:
- React State

**API Design**:
- RESTful

## 📋 Development Guidelines



## 📏 Coding Standards



## 📚 Required Libraries and Dependencies



## 🔒 Security Considerations



## ⚡ Performance Guidelines



## ✨ Best Practices

## 🧪 Testing Guidelines
  
  

## 🚀 Deployment Guidelines
  
  

## ⚠️ Critical Precautions



## 🛠️ Implementation Instructions

Build a responsive web application with modern frontend framework. Ensure cross-browser compatibility and accessibility.

### Development Workflow
1. **Setup**: Initialize project with proper structure and dependencies
2. **Core Implementation**: Build core functionality following architecture guidelines
3. **Security**: Implement security measures as outlined above
4. **Testing**: Write comprehensive tests for all components
5. **Performance**: Optimize based on performance guidelines
6. **Documentation**: Document all APIs, components, and deployment procedures
7. **Deployment**: Follow deployment guidelines for chosen platform

### Quality Checklist
- [ ] All security requirements implemented
- [ ] Performance optimizations applied
- [ ] Comprehensive test coverage achieved
- [ ] Code follows all coding standards
- [ ] Documentation is complete and accurate
- [ ] Deployment configuration is ready

---

## 📚 Final Notes

**Remember**: This prompt contains comprehensive guidelines for building a high-quality application. Prioritize security, performance, and maintainability throughout the development process.

**Code Quality**: Follow all coding standards and best practices outlined above.
**Security First**: Never compromise on security requirements.
**Performance**: Optimize early and measure continuously.
**Testing**: Maintain high test coverage and quality.

**Good luck with your development!** 🚀