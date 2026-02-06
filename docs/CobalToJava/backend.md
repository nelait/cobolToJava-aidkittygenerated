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
     ```json
     {
       "message": "Upload successful",
       "programId": "12345"
     }
     ```

2. **Extract Business Logic**
   - **Endpoint**: `/api/extract-logic/{programId}`
   - **Method**: GET
   - **Response**:
     ```json
     {
       "businessLogic": "...",
       "validations": "...",
       "externalAPIs": "..."
     }
     ```

3. **Generate Java Microservice**
   - **Endpoint**: `/api/generate-java-service/{programId}`
   - **Method**: POST
   - **Response**:
     ```json
     {
       "message": "Java microservice generated successfully",
       "serviceId": "67890"
     }
     ```

### Error Handling
- Standardize error responses with HTTP status codes and error messages:
  ```json
  {
    "error": "Invalid file format",
    "code": 400
  }
  ```

## Data Models

### Tables/Collections

1. **COBOLPrograms**
   - **Fields**:
     - `programId`: String (Primary Key)
     - `fileName`: String
     - `content`: Text
     - `uploadDate`: DateTime

2. **ExtractedLogic**
   - **Fields**:
     - `programId`: String (Foreign Key)
     - `businessLogic`: Text
     - `validations`: Text
     - `externalAPIs`: Text

3. **GeneratedServices**
   - **Fields**:
     - `serviceId`: String (Primary Key)
     - `programId`: String (Foreign Key)
     - `serviceCode`: Text
     - `generationDate`: DateTime

## Business Logic

- **Upload Process**: Validate file type and size, store file in database, assign a unique `programId`.
- **Extraction Process**: Parse COBOL code to extract business logic, validations, and external API calls. Store extracted information linked to `programId`.
- **Java Service Generation**: Convert extracted logic into Java Spring Boot code, generate service files, and store them.

## Security

- **Authentication**: Implement OAuth2 for secure access to all endpoints.
- **Authorization**: Ensure role-based access control (RBAC) to restrict access to certain endpoints.
- **Data Protection**: Use HTTPS for secure data transmission.

## Performance

- **File Processing**: Use asynchronous processing for file uploads to improve responsiveness.
- **Caching**: Implement caching for frequently accessed data such as extraction results.
- **Database Optimization**: Optimize database queries and indexing for faster data retrieval.

## Code Examples

### Sample COBOL Program Upload

```java
@RestController
@RequestMapping("/api")
public class CobolController {

    @PostMapping("/upload-cobol")
    public ResponseEntity<?> uploadCobol(@RequestParam("file") MultipartFile file) {
        try {
            String programId = cobolService.saveFile(file);
            return ResponseEntity.ok(Map.of("message", "Upload successful", "programId", programId));
        } catch (Exception e) {
            return ResponseEntity.status(HttpStatus.BAD_REQUEST).body(Map.of("error", e.getMessage()));
        }
    }
}
```

### Extract Business Logic

```java
@Service
public class CobolService {

    public String extractLogic(String programId) {
        // Load COBOL program from database
        COBOLProgram program = cobolRepository.findById(programId).orElseThrow();
        
        // Implement COBOL parsing logic here
        String businessLogic = parseBusinessLogic(program.getContent());
        
        // Save extracted logic to the database
        ExtractedLogic logic = new ExtractedLogic(programId, businessLogic, ...);
        extractedLogicRepository.save(logic);
        
        return businessLogic;
    }
}
```

---

This guide provides a structured approach to implementing the CobalToJava backend, ensuring a secure, scalable, and efficient system.
```