# CobalToJava Frontend Implementation Guide

This guide provides a detailed blueprint for implementing the frontend of the CobalToJava project. It covers the component structure, state management, UI/UX guidelines, and code examples to help you effectively build and integrate the required features.

## 1. Component Structure

### Main Components

1. **FileUploadComponent**
   - **Purpose**: To upload COBOL programs.
   - **Features**: Drag-and-drop area, file validation, progress indicator.

2. **ExtractionResultComponent**
   - **Purpose**: To display the extracted business logic, validations, and external APIs from COBOL programs.
   - **Features**: Tabbed view for different extraction categories, code highlighting.

3. **ServiceCreationComponent**
   - **Purpose**: To guide users in creating new Java Spring Boot microservices.
   - **Features**: Form for configuring service options, preview of generated code.

4. **AuthComponent**
   - **Purpose**: To handle OAuth integration.
   - **Features**: Login button, status indicator, user info display.

5. **NavigationComponent**
   - **Purpose**: To navigate between different sections of the application.
   - **Features**: Sidebar or top navigation bar.

### Component Hierarchy

```
App
 ├── NavigationComponent
 ├── AuthComponent
 ├── FileUploadComponent
 ├── ExtractionResultComponent
 └── ServiceCreationComponent
```

## 2. State Management

### Global State

Utilize a state management library such as Redux or Context API for managing global states. Key pieces of state include:

1. **AuthState**: Stores authentication tokens and user info.
   - Actions: `LOGIN`, `LOGOUT`, `SET_USER_INFO`

2. **FileUploadState**: Manages the state of uploaded files.
   - Actions: `UPLOAD_START`, `UPLOAD_SUCCESS`, `UPLOAD_FAILURE`

3. **ExtractionState**: Stores extracted information from COBOL programs.
   - Actions: `SET_EXTRACTION_RESULT`, `CLEAR_EXTRACTION_RESULT`

4. **ServiceCreationState**: Tracks service creation configurations.
   - Actions: `SET_SERVICE_CONFIG`, `RESET_SERVICE_CONFIG`

### Example Redux Configuration

```javascript
// actions.js
export const login = (token) => ({ type: 'LOGIN', payload: token });
export const uploadSuccess = (data) => ({ type: 'UPLOAD_SUCCESS', payload: data });

// reducers.js
const authReducer = (state = {}, action) => {
  switch (action.type) {
    case 'LOGIN':
      return { ...state, token: action.payload };
    default:
      return state;
  }
};

// store.js
import { createStore, combineReducers } from 'redux';
import authReducer from './reducers';

const rootReducer = combineReducers({
  auth: authReducer,
  // other reducers
});

const store = createStore(rootReducer);
```

## 3. UI/UX Guidelines

### Visual Design Considerations

1. **Consistency**: Maintain a consistent design language across components. Use a design system or component library like Material-UI or Ant Design.

2. **Accessibility**: Ensure all components are accessible. Use semantic HTML and ARIA attributes where necessary.

3. **Responsive Design**: Implement responsive design principles to accommodate different screen sizes, especially for file upload and extraction result components.

4. **User Feedback**: Provide immediate and clear feedback for actions, such as uploading files or generating services.

### Styling

- **Color Scheme**: A professional and simple color palette with primary, secondary, and accent colors.
- **Typography**: Use a readable font with appropriate size and weight for headings and body text.

## 4. Code Examples

### FileUploadComponent

```jsx
import React, { useState } from 'react';

const FileUploadComponent = () => {
  const [file, setFile] = useState(null);

  const handleFileChange = (event) => {
    setFile(event.target.files[0]);
  };

  const handleUpload = () => {
    // Dispatch upload action
  };

  return (
    <div className="file-upload">
      <input type="file" onChange={handleFileChange} />
      <button onClick={handleUpload}>Upload</button>
    </div>
  );
};

export default FileUploadComponent;
```

### ExtractionResultComponent

```jsx
import React from 'react';

const ExtractionResultComponent = ({ extractionData }) => {
  return (
    <div className="extraction-result">
      <h2>Extraction Results</h2>
      <div className="tabs">
        {/* Map through extraction categories */}
        {extractionData.map((category, index) => (
          <div key={index} className="tab-content">
            <h3>{category.title}</h3>
            <pre>{category.content}</pre>
          </div>
        ))}
      </div>
    </div>
  );
};

export default ExtractionResultComponent;
```

This guide should serve as a comprehensive starting point for implementing the frontend of the CobalToJava project. Adjust and expand upon these guidelines as needed to fit the specific requirements and constraints of your development environment.