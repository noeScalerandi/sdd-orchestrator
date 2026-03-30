# 🤖 AI Agent Feature/Task Brief (Derived from Jira)

## 1. Feature/Task Metadata

- **Ticket ID:** HELLO-001
- **Title:** Hello World TypeScript React Component
- **Type:** Feature
- **Owner (if any):** Product Team

---

## 2. Feature/Task Summary (Plain Language)

Create a new React component written in TypeScript using the latest version of React. The component renders a simple "Hello World" message on screen. It should follow React best practices, including functional component style with proper TypeScript typing.

> _This component serves as a foundational building block and demonstrates the project setup with React and TypeScript._

---

## 3. Goal / Expected Outcome

Define exactly what success looks like.

- Primary outcome: A working React functional component written in TypeScript that displays "Hello World"
- Secondary outcomes (if any): Component is reusable, properly typed, and follows React best practices
- Definition of done: The component renders "Hello World" text in the browser without errors, and passes TypeScript type checks

---

## 4. Execution Instructions (Step-by-Step)

Provide **explicit, ordered steps** the agent must follow.

1. Create a new TypeScript file at `src/components/HelloWorld.tsx`
2. Define a functional React component named `HelloWorld` using the `React.FC` type (or equivalent modern React typing)
3. The component must render a `<p>` (or `<h1>`) element containing the text `"Hello World"`
4. Export the component as the default export
5. Ensure the component compiles without TypeScript errors

> ⚠️ Be precise. Use the latest stable version of React (React 19+). Do not use class components.

---

## 5. Constraints & Rules

Define boundaries the agent must respect.

- Do NOT: Use class-based components
- Do NOT: Use JavaScript — all code must be TypeScript (`.tsx`)
- Must: Use functional component syntax
- Must: Use the latest stable version of React available
- Limitations (tech, business, security): No external UI libraries; only React and TypeScript
- Assumptions: The project is a standard React + TypeScript application (e.g., created with Vite or Create React App with TypeScript template)

---

## 6. Context & Background

Provide only relevant context needed to complete the task.

- Business context: This component is a starter template for demonstrating React + TypeScript integration
- User impact: Developers will use this as a reference point for creating new components
- Related components / systems: Can be integrated into the root `App.tsx` component
- Dependencies: React (latest stable), TypeScript

---

## 7. Inputs

All resources the agent should use.

- **Documents / links:** [React official docs](https://react.dev), [TypeScript handbook](https://www.typescriptlang.org/docs/)
- **APIs / endpoints:** N/A
- **Schemas / data models:** N/A
- **Sample inputs:** No props required for this component

---

## 8. Expected Output Format

Be explicit about how the agent should respond.

- Format: TypeScript/React code file (`.tsx`)
- Structure: Single functional component with default export

Example:

```tsx
import React from 'react';

const HelloWorld: React.FC = () => {
  return <p>Hello World</p>;
};

export default HelloWorld;
```
