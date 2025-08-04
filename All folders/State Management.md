> **State management** is how your app **keeps track of and updates data** (called “state”) that changes over time — like user input, login status, selected items, etc.

- Or in other words it can be described as Handling data inside frontend

It helps your app know **what to show** and **when to update the UI** when something changes.

---

###  Example (Think of your LMS):

|What Changes|Why It's State|
|---|---|
|User logs in|Now the app should show their profile instead of the login page|
|Student selects a course|The app should now show the selected course content|
|A quiz is submitted|The UI needs to show the score and feedback|
### Where Can State Live?

There are **three main types** of state in a frontend app (especially in React):

| Type             | Example                                 | Where it Lives                                        |
| ---------------- | --------------------------------------- | ----------------------------------------------------- |
| **Local State**  | Form input, toggle switch               | Inside a component (`useState`)                       |
| **Global State** | Logged-in user info, theme (dark/light) | Across many components (Context, Redux)               |
| **Server State** | Data from an API (courses, scores)      | Fetched from backend (React Query, Axios + useEffect) |
###  Tools for State Management in React:

| Tool                         | Use Case                                       |
| ---------------------------- | ---------------------------------------------- |
| `useState`                   | For local state inside one component           |
| `useContext`                 | Share state across multiple components         |
| **Redux / Zustand / Recoil** | For large-scale apps with complex state        |
| `React Query` / `SWR`        | For server data (loading, caching, refetching) |