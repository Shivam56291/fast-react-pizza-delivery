# 🍕 Fast React Pizza Co.

A modern single-page pizza ordering web application built with **React 18**, **React Router v6.14**, **Redux Toolkit**, and **Tailwind CSS**, bundled with **Vite** for blazing-fast development and builds.  

👉 [Live Demo](https://fast-react-pizza-delivery-co.netlify.app/)  

---

## ✨ Features

- 📋 **Browse Menu** – Dynamic pizza menu fetched using React Router loaders.  
- 🛒 **Cart Management** – Add, update, and remove pizzas with Redux Toolkit.  
- 📝 **Place Orders** – Submit validated orders via React Router actions.  
- 🚚 **Track Orders** – Real-time delivery tracking with estimated time.  
- 📍 **Geolocation Integration** – Auto-fetch user’s address with reverse geocoding API + async thunk.  
- ⚡ **Priority Orders** – Option to prioritize orders with updated price.  
- 🎨 **Responsive UI** – Tailwind CSS for modern and adaptive styling.  

---

## 🛠️ Tech Stack

- **Frontend**: React 18, React Router v6.14, Redux Toolkit, Tailwind CSS  
- **Build Tool**: Vite  
- **Data Handling**: React Router **Loaders**, **Actions**, `useFetcher`  
- **State Management**: Redux Toolkit slices (`cart`, `user`)  
- **Async Handling**: Redux `createAsyncThunk` for geolocation & APIs  
- **Styling**: Tailwind utility classes + custom responsive UI  

---

## 📂 Project Structure

```
src/
├── features/
│ ├── cart/ # Cart slice, UI, and logic
│ ├── menu/ # Menu loader and menu UI
│ ├── order/ # Order creation, actions, and tracking
│ └── user/ # User slice, async thunk for geolocation
├── services/ # API abstraction (apiRestaurant.js)
├── ui/ # Reusable UI components (Button, Layout, etc.)
├── utils/ # Helper functions (formatCurrency, dates, etc.)
└── App.jsx # Router setup with nested routes

```



---

## ⚛️ React Concepts & Hooks Used

This project demonstrates **modern React best practices** with the following hooks and concepts:  

- **React Core Hooks**
  - `useState` – local state management  
  - `useEffect` – side effects & subscriptions  
  - `useRef` – managing DOM references & persisting values  
  - `useReducer` – (for more complex state in some components)  
  - `useMemo` – memoized values for performance  
  - `useCallback` – memoized functions to prevent re-renders  

- **React Router Hooks**
  - `useLoaderData` – access loader-fetched data  
  - `useActionData` – access action return values (form submissions)  
  - `useFetcher` – handle background fetches without navigation  
  - `useNavigation` – loading states during navigation  
  - `useParams` – read route parameters (e.g., order ID)  
  - `useNavigate` – programmatic navigation  

- **Redux Toolkit**
  - `useSelector` – read state from slices  
  - `useDispatch` – dispatch actions  
  - `createSlice` – feature-based state slices (`cart`, `user`)  
  - `createAsyncThunk` – async side effects (geolocation API)  

- **Other React Patterns**
  - Controlled & uncontrolled components  
  - Form validation & error handling via actions  
  - Global state via Redux vs local state via React  
  - Feature-based folder structure for scalability  

---

## 🧑‍💻 Code Concepts Demonstrated

- **Redux Toolkit Slices** → cart management, user address  
- **Async Thunks** → fetch geolocation + reverse geocoding  
- **React Router Loaders** → menu fetching, order tracking  
- **React Router Actions** → order creation via form submission  
- **Reusable Components** → Button, Input, Layout, Loader  
- **Responsive UI** → Tailwind utility-first styling  
- **Conditional Rendering** → loaders, error messages, states  
- **Error Handling** → router errorElement + custom messages  

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/fast-react-pizza.git
cd fast-react-pizza
```

### 2. Install dependencies
```
npm install
```

### 3. Run the development server
```
npm run dev
```

### 4. Build for production
```
npm run build
```

## 🧪 Key Learnings (from building this project)

 - Leveraging React Router loaders & actions for async data fetching and mutations.

 - Managing global app state effectively with Redux Toolkit slices.

 - Using async thunks for geolocation and external API integration.

 - Designing reusable, responsive UI components with Tailwind CSS.

 - Structuring a scalable React app with a feature-based architecture.

 - Balancing local state vs global state in modern React apps.
