# 🤖 AI Agent Feature/Task Brief (Derived from Jira)

## 1. Feature/Task Metadata

- **Ticket ID:** HELLO-001
- **Title:** Hello World React TypeScript Component
- **Type:** Feature
- **Owner (if any):** N/A

---

## 2. Feature/Task Summary (Plain Language)

Create a new React component written in TypeScript using the latest version of React (React 19). The component should render a simple "Hello World" message. This serves as a minimal, working example of a typed React functional component.

> _This component is a self-contained UI unit that displays a static "Hello World" text. It requires no external data, no API calls, and no state management._

---

## 3. Goal / Expected Outcome

Define exactly what success looks like.

- Primary outcome: A reusable, type-safe React 19 functional component that renders "Hello World"
- Secondary outcomes (if any): Serves as a reference implementation for typed React components in this project
- Definition of done: The component file exists at `src/components/HelloWorld.tsx`, compiles without TypeScript errors, and renders the text "Hello World" when mounted

---

## 4. Execution Instructions (Step-by-Step)

Provide **explicit, ordered steps** the agent must follow.

1. Create the file `src/components/HelloWorld.tsx`
2. Implement a React 19 functional component named `HelloWorld` (no explicit `React.FC` type needed)
3. Render a `<div>` element containing the text "Hello World"
4. Export the component as the default export
5. Do NOT add a `React` import — React 19's JSX transform does not require it

> ⚠️ Be precise. Avoid vague instructions.

---

## 5. Constraints & Rules

Define boundaries the agent must respect.

- Do NOT use `any` TypeScript type — all types must be explicit
- Do NOT use class components — use functional components only
- Do NOT import `React` explicitly — React 19's new JSX transform handles this automatically
- Do NOT use `React.FC` — use plain arrow function syntax for components
- Must use React 19 (latest version)
- Must be written in TypeScript (`.tsx` extension)
- Limitations: No external dependencies beyond `react` and `react-dom`
- Assumptions: The project uses TypeScript strict mode and the new JSX transform (`"jsx": "react-jsx"` in `tsconfig.json`)

---

## 6. Context & Background

Provide only relevant context needed to complete the task.

- Business context: This is a minimal example component to demonstrate TypeScript + React 19 integration
- User impact: Developers can use this as a reference for creating new components in the project
- Related components / systems: None
- Dependencies: `react` ^19.0.0, `@types/react` ^19.0.0

---

## 7. Inputs

All resources the agent should use.

- **Documents / links:** [React 19 documentation](https://react.dev)
- **APIs / endpoints:** N/A
- **Schemas / data models:** N/A
- **Sample inputs:** N/A

---

## 8. Expected Output Format

Be explicit about how the agent should respond.

- Format: TypeScript React component file (`.tsx`)
- Structure: Functional component with typed props interface, default export

Example:

```tsx
const HelloWorld = () => {
  return <div>Hello World</div>;
};

export default HelloWorld;
```
