# Front-End Developer Technical Assessment

## Overview
Welcome to our Front-End Developer Technical Assessment! This challenge is designed to evaluate your ability to:
- Recreate a given **UI component** with attention to detail
- Handle **data fetching** efficiently
- Implement a **form submission workflow** with API integration
- Ensure **responsiveness, accessibility, and UX micro-interactions**
- Write **clean, modular, and maintainable code**

You are free to use **any front-end framework or vanilla JavaScript**. The goal is to see **your approach and problem-solving skills** rather than enforce a specific tech stack. That being said, we generally use Nuxt/Vue & Tailwind in-house, but again no pressure!

---

## 📌 Requirements

### 1️⃣ UI Component Replication (Attention to Detail & Design System)
Create a visually polished User Profile Card component that is compact yet spacious, minimal yet bold, and uses subtle but noticeable icons for additional actions.

### **Component Requirements:**
- **Circular avatar image** at the top.
- **Full name** and **email** included.
- **Country badge**.
- **Flag icon** in the top-right corner that toggles on/off when clicked.
- **Primary button** (e.g., "View Profile") with a hover effect.
- **Consistent spacing, typography, and responsiveness**.

🔹 **Bonus Points**:
- Implement **dark mode support**.
- Add **micro-interactions (hover, animations, loading states, etc.)**.

---

### 2️⃣ Data Fetching & State Management
Fetch user data dynamically from an API and display multiple **Profile Cards** in a comfortable layout.

#### **API Endpoint:**
`https://randomuser.me/api/?results=10`

#### **Requirements:**
- Fetch **10 random users** and render their details inside the **User Profile Card**.
- Ensure the UI **updates smoothly** when fetching new data.
- Use **state management** (React Context, Zustand, Vue Pinia, or a similar approach).
- Handle **loading, success, and error states gracefully**.

🔹 **Bonus Points**:
- Implement **lazy loading** for avatars/images.
- Use a **debounced API call** to prevent unnecessary requests.

---

### 3️⃣ Flag Logic & API Integration
Each User Profile Card should include a "Flag" icon/button in the upper-right corner. Clicking this should send a POST request to our backend API (Directus) with the user’s data. Handle API success, errors, and prevent duplicate flagging.

#### Requirements
- Each User Profile Card must have a “flag” icon/button in the upper-right corner.
- Clicking fires a POST request with the user’s data to our backend API.
- The flag icon should visually differ between flagged/not-flagged states.
- Prevent duplicate flagging (e.g., disable button after submission).

 
#### **Directus API Endpoint (open; no auth required):**
```
POST https://mlabs.directus.app/items/fe_flagged_users
Body (example):
{
  "photo_url": "https://randomuser.me/api/portraits/men/1.jpg",
  "first_name": "John",
  "last_name": "Doe",
  "email": "john.doe@example.com",
  "country": "United States"
}
```

---

## 📂 Submission Guidelines
1. **Fork this repo** and complete the assignment in your own repository.
2. **Push incremental commits** (we'll check commit history for logical progress).
3. **Submit your final GitHub repo link**.

🔹 **Bonus:** Attach a short **README write-up** explaining your approach.

---

## 🚀 Extra Opportunities
✅ **Dark mode support**  
✅ **Lazy loading for avatars**  
✅ **Animations & transitions**  
✅ **Ensuring accessibility & keyboard navigation**  

---

## ⚠️ Important Notes
- We care more about **your thought process and execution** than just the final code.

Reach out with any questions or concerns as needed!
