# **Fitness Tracker Application - Challenge 05**

## **Description**
This is a fitness tracking application built using **React**, **TypeScript**, and **Firebase**. The app allows users to log in with Google, track their workouts, and manage their fitness data. Firebase Firestore is used for data storage, and Firebase Authentication ensures secure login.

## **Features**

### **Main Components**
- **Welcome Page**
  - Displays a hero banner for unauthenticated users.
  - Includes a **Google Sign-In** button.
  - Authentication is handled using Firebase `signInWithPopup`.

- **Navbar**
  - Visible on all pages except the **Welcome Page**.
  - The **logo** links to **All Workouts**.
  - The **plus icon** links to **Add New Workout**.
  - The **Logout** button calls `signOut` and redirects to the **Welcome Page**.

- **AllWorkouts**
  - Displays a list of all workouts from Firestore.
  - If no workouts are available, it shows a message: **"There are no workouts."**

- **AddNewWorkout**
  - A form to add a new workout.
  - Includes fields for **exercise type, duration, and intensity**.
  - The **exercise types** are fetched from `workoutTypes.json` and displayed as select options.
  - **Intensity options**: "Low", "Medium", or "High".
  - Validates input before saving the workout to Firestore.

---

## **Technologies Used**
- **React (TypeScript)**
- **Material-UI** (for styling)
- **Firebase Authentication** (Google Sign-In)
- **Firestore Database** (for workouts)
- **Firebase Hosting** (for deployment)
- **React Router** (for navigation)
- **Context API** (for global authentication state)



