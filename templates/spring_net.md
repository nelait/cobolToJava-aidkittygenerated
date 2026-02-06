# spring.net



**Application Type:** web
**Category:** fullstack
**Tags:** springboot

## Architecture
{
  "pattern": "Full-stack monorepo or separate repos, API-first design approach, Shared type definitions, Microservices or monolithic architecture",
  "description": "Application architecture pattern",
  "structure": {
    "directories": [
      "Full-stack monorepo or separate repos",
      "API-first design approach",
      "Shared type definitions",
      "Microservices or monolithic architecture"
    ],
    "files": [
      "Client-server communication patterns",
      "Database to API to frontend flow",
      "Real-time updates (WebSockets, SSE)",
      "Caching strategies across layers"
    ],
    "conventions": [
      "File-based routing (Next.js style)",
      "API route organization",
      "Protected routes and middleware",
      "SEO-friendly routing"
    ]
  },
  "dataFlow": "Client-server communication patterns, Database to API to frontend flow, Real-time updates (WebSockets, SSE), Caching strategies across layers",
  "stateManagement": "React State",
  "apiDesign": "RESTful"
}

## Guidelines
[
  {
    "title": "Use modern full-stack framework (Next.js, Nuxt.js, SvelteKit)",
    "description": "Use modern full-stack framework (Next.js, Nuxt.js, SvelteKit)",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Implement proper client-server separation",
    "description": "Implement proper client-server separation",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Use server-side rendering where appropriate",
    "description": "Use server-side rendering where appropriate",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Follow full-stack best practices",
    "description": "Follow full-stack best practices",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Organize by feature or domain",
    "description": "Organize by feature or domain",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Separate client and server logic clearly",
    "description": "Separate client and server logic clearly",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Use shared types and utilities",
    "description": "Use shared types and utilities",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Implement proper API layer structure",
    "description": "Implement proper API layer structure",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Optimize both client and server performance",
    "description": "Optimize both client and server performance",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Implement proper caching strategies",
    "description": "Implement proper caching strategies",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Use CDN for static assets",
    "description": "Use CDN for static assets",
    "priority": "medium",
    "examples": []
  },
  {
    "title": "Optimize database queries and API calls",
    "description": "Optimize database queries and API calls",
    "priority": "medium",
    "examples": []
  }
]

## Standards
[
  {
    "name": "Use consistent naming across frontend and backend",
    "description": "Use consistent naming across frontend and backend",
    "type": "naming",
    "rules": [
      "Use consistent naming across frontend and backend"
    ],
    "examples": []
  },
  {
    "name": "Follow framework-specific conventions",
    "description": "Follow framework-specific conventions",
    "type": "naming",
    "rules": [
      "Follow framework-specific conventions"
    ],
    "examples": []
  },
  {
    "name": "Use descriptive API endpoint names",
    "description": "Use descriptive API endpoint names",
    "type": "naming",
    "rules": [
      "Use descriptive API endpoint names"
    ],
    "examples": []
  },
  {
    "name": "Maintain consistent file naming",
    "description": "Maintain consistent file naming",
    "type": "naming",
    "rules": [
      "Maintain consistent file naming"
    ],
    "examples": []
  },
  {
    "name": "Use Prettier for both frontend and backend",
    "description": "Use Prettier for both frontend and backend",
    "type": "formatting",
    "rules": [
      "Use Prettier for both frontend and backend"
    ],
    "examples": []
  },
  {
    "name": "Configure ESLint for full-stack consistency",
    "description": "Configure ESLint for full-stack consistency",
    "type": "formatting",
    "rules": [
      "Configure ESLint for full-stack consistency"
    ],
    "examples": []
  },
  {
    "name": "Use consistent indentation across projects",
    "description": "Use consistent indentation across projects",
    "type": "formatting",
    "rules": [
      "Use consistent indentation across projects"
    ],
    "examples": []
  },
  {
    "name": "Follow framework formatting conventions",
    "description": "Follow framework formatting conventions",
    "type": "formatting",
    "rules": [
      "Follow framework formatting conventions"
    ],
    "examples": []
  },
  {
    "name": "Document API endpoints with OpenAPI",
    "description": "Document API endpoints with OpenAPI",
    "type": "documentation",
    "rules": [
      "Document API endpoints with OpenAPI"
    ],
    "examples": []
  },
  {
    "name": "Maintain component and function documentation",
    "description": "Maintain component and function documentation",
    "type": "documentation",
    "rules": [
      "Maintain component and function documentation"
    ],
    "examples": []
  },
  {
    "name": "Document database schema and migrations",
    "description": "Document database schema and migrations",
    "type": "documentation",
    "rules": [
      "Document database schema and migrations"
    ],
    "examples": []
  },
  {
    "name": "Keep deployment and setup documentation updated",
    "description": "Keep deployment and setup documentation updated",
    "type": "documentation",
    "rules": [
      "Keep deployment and setup documentation updated"
    ],
    "examples": []
  }
]

## Libraries
[
  {
    "name": "Next.js or Nuxt.js for full-stack framework",
    "description": "Next.js or Nuxt.js for full-stack framework",
    "version": "latest",
    "category": "core",
    "required": true,
    "installation": "npm install Next.js or Nuxt.js for full-stack framework",
    "usage": "Next.js or Nuxt.js for full-stack framework",
    "alternatives": []
  },
  {
    "name": "TypeScript for type safety across stack",
    "description": "TypeScript for type safety across stack",
    "version": "latest",
    "category": "core",
    "required": true,
    "installation": "npm install TypeScript for type safety across stack",
    "usage": "TypeScript for type safety across stack",
    "alternatives": []
  },
  {
    "name": "Database ORM (Prisma, Drizzle)",
    "description": "Database ORM (Prisma, Drizzle)",
    "version": "latest",
    "category": "core",
    "required": true,
    "installation": "npm install Database ORM (Prisma, Drizzle)",
    "usage": "Database ORM (Prisma, Drizzle)",
    "alternatives": []
  },
  {
    "name": "Authentication library (NextAuth, Supabase)",
    "description": "Authentication library (NextAuth, Supabase)",
    "version": "latest",
    "category": "core",
    "required": true,
    "installation": "npm install Authentication library (NextAuth, Supabase)",
    "usage": "Authentication library (NextAuth, Supabase)",
    "alternatives": []
  },
  {
    "name": "Tailwind CSS for styling",
    "description": "Tailwind CSS for styling",
    "version": "latest",
    "category": "ui",
    "required": false,
    "installation": "npm install Tailwind CSS for styling",
    "usage": "Tailwind CSS for styling",
    "alternatives": []
  },
  {
    "name": "Component library (Radix, Headless UI)",
    "description": "Component library (Radix, Headless UI)",
    "version": "latest",
    "category": "ui",
    "required": false,
    "installation": "npm install Component library (Radix, Headless UI)",
    "usage": "Component library (Radix, Headless UI)",
    "alternatives": []
  },
  {
    "name": "Form handling (React Hook Form)",
    "description": "Form handling (React Hook Form)",
    "version": "latest",
    "category": "ui",
    "required": false,
    "installation": "npm install Form handling (React Hook Form)",
    "usage": "Form handling (React Hook Form)",
    "alternatives": []
  },
  {
    "name": "State management (Zustand, Redux Toolkit)",
    "description": "State management (Zustand, Redux Toolkit)",
    "version": "latest",
    "category": "ui",
    "required": false,
    "installation": "npm install State management (Zustand, Redux Toolkit)",
    "usage": "State management (Zustand, Redux Toolkit)",
    "alternatives": []
  },
  {
    "name": "Validation library (Zod, Yup)",
    "description": "Validation library (Zod, Yup)",
    "version": "latest",
    "category": "utilities",
    "required": false,
    "installation": "npm install Validation library (Zod, Yup)",
    "usage": "Validation library (Zod, Yup)",
    "alternatives": []
  },
  {
    "name": "Date manipulation (date-fns)",
    "description": "Date manipulation (date-fns)",
    "version": "latest",
    "category": "utilities",
    "required": false,
    "installation": "npm install Date manipulation (date-fns)",
    "usage": "Date manipulation (date-fns)",
    "alternatives": []
  },
  {
    "name": "HTTP client (Axios, fetch)",
    "description": "HTTP client (Axios, fetch)",
    "version": "latest",
    "category": "utilities",
    "required": false,
    "installation": "npm install HTTP client (Axios, fetch)",
    "usage": "HTTP client (Axios, fetch)",
    "alternatives": []
  },
  {
    "name": "Environment configuration (dotenv)",
    "description": "Environment configuration (dotenv)",
    "version": "latest",
    "category": "utilities",
    "required": false,
    "installation": "npm install Environment configuration (dotenv)",
    "usage": "Environment configuration (dotenv)",
    "alternatives": []
  }
]

## Security
[
  {
    "title": "Implement secure authentication flow",
    "description": "Implement secure authentication flow",
    "threat": "Authentication",
    "priority": "high",
    "mitigation": [
      "Implement secure authentication flow"
    ],
    "tools": []
  },
  {
    "title": "Use JWT tokens with proper expiration",
    "description": "Use JWT tokens with proper expiration",
    "threat": "Authentication",
    "priority": "high",
    "mitigation": [
      "Use JWT tokens with proper expiration"
    ],
    "tools": []
  },
  {
    "title": "Implement proper session management",
    "description": "Implement proper session management",
    "threat": "Authentication",
    "priority": "high",
    "mitigation": [
      "Implement proper session management"
    ],
    "tools": []
  },
  {
    "title": "Validate and sanitize user inputs",
    "description": "Validate and sanitize user inputs",
    "threat": "Data Protection",
    "priority": "high",
    "mitigation": [
      "Validate and sanitize user inputs"
    ],
    "tools": []
  },
  {
    "title": "Implement CSRF protection",
    "description": "Implement CSRF protection",
    "threat": "Data Protection",
    "priority": "high",
    "mitigation": [
      "Implement CSRF protection"
    ],
    "tools": []
  },
  {
    "title": "Use HTTPS for all communications",
    "description": "Use HTTPS for all communications",
    "threat": "Data Protection",
    "priority": "high",
    "mitigation": [
      "Use HTTPS for all communications"
    ],
    "tools": []
  },
  {
    "title": "Regularly update dependencies",
    "description": "Regularly update dependencies",
    "threat": "Dependencies",
    "priority": "medium",
    "mitigation": [
      "Regularly update dependencies"
    ],
    "tools": []
  },
  {
    "title": "Use npm audit for security vulnerabilities",
    "description": "Use npm audit for security vulnerabilities",
    "threat": "Dependencies",
    "priority": "medium",
    "mitigation": [
      "Use npm audit for security vulnerabilities"
    ],
    "tools": []
  },
  {
    "title": "Implement dependency scanning in CI/CD",
    "description": "Implement dependency scanning in CI/CD",
    "threat": "Dependencies",
    "priority": "medium",
    "mitigation": [
      "Implement dependency scanning in CI/CD"
    ],
    "tools": []
  }
]

## Performance
[
  {
    "title": "Implement code splitting at route level",
    "description": "Implement code splitting at route level",
    "impact": "medium",
    "optimization": [
      "Implement code splitting at route level"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Use React.lazy for component lazy loading",
    "description": "Use React.lazy for component lazy loading",
    "impact": "medium",
    "optimization": [
      "Use React.lazy for component lazy loading"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Optimize bundle size with tree shaking",
    "description": "Optimize bundle size with tree shaking",
    "impact": "medium",
    "optimization": [
      "Optimize bundle size with tree shaking"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Use React DevTools for debugging",
    "description": "Use React DevTools for debugging",
    "impact": "medium",
    "optimization": [
      "Use React DevTools for debugging"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Implement error tracking (Sentry)",
    "description": "Implement error tracking (Sentry)",
    "impact": "medium",
    "optimization": [
      "Implement error tracking (Sentry)"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Monitor Core Web Vitals",
    "description": "Monitor Core Web Vitals",
    "impact": "medium",
    "optimization": [
      "Monitor Core Web Vitals"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Implement loading states for async operations",
    "description": "Implement loading states for async operations",
    "impact": "medium",
    "optimization": [
      "Implement loading states for async operations"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Use skeleton screens for better UX",
    "description": "Use skeleton screens for better UX",
    "impact": "medium",
    "optimization": [
      "Use skeleton screens for better UX"
    ],
    "metrics": [],
    "tools": []
  },
  {
    "title": "Optimize images with lazy loading",
    "description": "Optimize images with lazy loading",
    "impact": "medium",
    "optimization": [
      "Optimize images with lazy loading"
    ],
    "metrics": [],
    "tools": []
  }
]

## Testing
[
  {
    "type": "unit",
    "framework": "jest",
    "description": "Use Jest and React Testing Library",
    "coverage": "80%",
    "examples": [
      "Use Jest and React Testing Library"
    ]
  },
  {
    "type": "unit",
    "framework": "jest",
    "description": "Test component behavior, not implementation",
    "coverage": "80%",
    "examples": [
      "Test component behavior, not implementation"
    ]
  },
  {
    "type": "unit",
    "framework": "jest",
    "description": "Aim for 80%+ code coverage",
    "coverage": "80%",
    "examples": [
      "Aim for 80%+ code coverage"
    ]
  },
  {
    "type": "integration",
    "framework": "jest",
    "description": "Test user workflows and interactions",
    "coverage": "70%",
    "examples": [
      "Test user workflows and interactions"
    ]
  },
  {
    "type": "integration",
    "framework": "jest",
    "description": "Test API integrations",
    "coverage": "70%",
    "examples": [
      "Test API integrations"
    ]
  },
  {
    "type": "integration",
    "framework": "jest",
    "description": "Use MSW for API mocking",
    "coverage": "70%",
    "examples": [
      "Use MSW for API mocking"
    ]
  },
  {
    "type": "e2e",
    "framework": "cypress",
    "description": "Use Cypress or Playwright for E2E tests",
    "coverage": "60%",
    "examples": [
      "Use Cypress or Playwright for E2E tests"
    ]
  },
  {
    "type": "e2e",
    "framework": "cypress",
    "description": "Test critical user journeys",
    "coverage": "60%",
    "examples": [
      "Test critical user journeys"
    ]
  },
  {
    "type": "e2e",
    "framework": "cypress",
    "description": "Run tests in CI/CD pipeline",
    "coverage": "60%",
    "examples": [
      "Run tests in CI/CD pipeline"
    ]
  }
]

## Deployment
[
  {
    "platform": "build",
    "description": "Configure build optimization",
    "steps": [
      "Configure build optimization"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "build",
    "description": "Implement environment-specific builds",
    "steps": [
      "Implement environment-specific builds"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "build",
    "description": "Use build caching for faster deployments",
    "steps": [
      "Use build caching for faster deployments"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "hosting",
    "description": "Deploy to Vercel, Netlify, or AWS",
    "steps": [
      "Deploy to Vercel, Netlify, or AWS"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "hosting",
    "description": "Configure proper redirects and rewrites",
    "steps": [
      "Configure proper redirects and rewrites"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "hosting",
    "description": "Set up CDN for static assets",
    "steps": [
      "Set up CDN for static assets"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "cicd",
    "description": "Set up automated testing in CI/CD",
    "steps": [
      "Set up automated testing in CI/CD"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "cicd",
    "description": "Implement automated deployments",
    "steps": [
      "Implement automated deployments"
    ],
    "configuration": [],
    "monitoring": []
  },
  {
    "platform": "cicd",
    "description": "Use feature flags for gradual rollouts",
    "steps": [
      "Use feature flags for gradual rollouts"
    ],
    "configuration": [],
    "monitoring": []
  }
]

## Precautions
[
  {
    "title": "Avoid prop drilling - use Context or state management",
    "description": "Avoid prop drilling - use Context or state management",
    "severity": "medium",
    "prevention": [
      "Avoid prop drilling - use Context or state management"
    ]
  },
  {
    "title": "Prevent memory leaks with proper cleanup",
    "description": "Prevent memory leaks with proper cleanup",
    "severity": "medium",
    "prevention": [
      "Prevent memory leaks with proper cleanup"
    ]
  },
  {
    "title": "Handle edge cases and error states",
    "description": "Handle edge cases and error states",
    "severity": "medium",
    "prevention": [
      "Handle edge cases and error states"
    ]
  },
  {
    "title": "Avoid unnecessary re-renders",
    "description": "Avoid unnecessary re-renders",
    "severity": "medium",
    "prevention": [
      "Avoid unnecessary re-renders"
    ]
  },
  {
    "title": "Be careful with useEffect dependencies",
    "description": "Be careful with useEffect dependencies",
    "severity": "medium",
    "prevention": [
      "Be careful with useEffect dependencies"
    ]
  },
  {
    "title": "Optimize expensive computations with useMemo",
    "description": "Optimize expensive computations with useMemo",
    "severity": "medium",
    "prevention": [
      "Optimize expensive computations with useMemo"
    ]
  },
  {
    "title": "Validate all user inputs",
    "description": "Validate all user inputs",
    "severity": "high",
    "prevention": [
      "Validate all user inputs"
    ]
  },
  {
    "title": "Avoid XSS vulnerabilities",
    "description": "Avoid XSS vulnerabilities",
    "severity": "high",
    "prevention": [
      "Avoid XSS vulnerabilities"
    ]
  },
  {
    "title": "Implement proper authentication and authorization",
    "description": "Implement proper authentication and authorization",
    "severity": "high",
    "prevention": [
      "Implement proper authentication and authorization"
    ]
  }
]
