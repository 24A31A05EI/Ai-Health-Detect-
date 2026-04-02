# 🏥 AI Health Detect System

---

## 📌 Project Description

AI Health Detect System is an AI-powered web application that enables users to predict their risk for multiple serious diseases — Diabetes, Heart Disease, Kidney Disease, and Cancer — by entering key health metrics. It provides instant risk assessments with confidence scores and maintains a personal health records history, all within a clean and responsive interface.

---

## ❗ Problem Statement

Millions of people worldwide are unaware of their risk for life-threatening diseases until it is too late. Early detection is critical, yet access to medical screening is often costly, time-consuming, or geographically limited. There is a strong need for an accessible, easy-to-use digital tool that allows individuals to assess their health risk quickly using basic clinical data — empowering them to take timely action and consult medical professionals early.

---

## ✨ Features

- **Multi-Disease Prediction** — Risk assessment for four diseases: Diabetes, Heart Disease, Kidney Disease, and Cancer.
- **AI Risk Scoring** — Each prediction returns a risk score (0–100%), a confidence level, and a classification (Low / Moderate / High).
- **User Authentication** — Secure Sign Up, Login, and Password Reset flows with protected routes.
- **Personal Health Records** — All prediction results are saved locally and viewable in a dedicated Records page.
- **Interactive Dashboard** — Overview of recent activity and prediction summaries.
- **Research Page** — Curated health and disease research references for user education.
- **User Profile & Settings** — Manage account details and app preferences.
- **Dark / Light Theme** — Toggle between themes, with preference persisted across sessions.
- **Responsive Design** — Fully functional across desktop and mobile screens.
- **Toast Notifications** — Real-time feedback on actions and errors.
- **Error Boundaries** — Graceful fallback UI for unexpected runtime errors.

---

## 🛠️ Technology Used

| Category | Tool / Language |
|---|---|
| **Frontend Framework** | React 19 |
| **Language** | TypeScript |
| **Build Tool** | Vite |
| **Styling** | Tailwind CSS v4 |
| **Routing** | React Router DOM v7 |
| **State Management** | Zustand |
| **Form Handling** | React Hook Form |
| **Schema Validation** | Zod |
| **Animation** | Framer Motion |
| **Charts / Visualization** | Recharts |
| **Icons** | Lucide React, Heroicons |
| **UI Primitives** | Radix UI (Dropdown Menu) |
| **Data Persistence** | localStorage (via UUID-keyed records) |
| **Linting** | ESLint, TypeScript ESLint |
| **Formatting** | Prettier |

---

## 📁 Project Structure

```
Ai-Health-Detect-System-main/
├── public/
│   ├── favicon.svg
│   └── icons.svg
├── src/
│   ├── assets/                  # Static assets (images, SVGs)
│   ├── components/              # Reusable UI components
│   │   ├── ErrorBoundary.tsx
│   │   ├── Navbar.tsx
│   │   ├── ProtectedRoute.tsx
│   │   ├── Sidebar.tsx
│   │   └── Toast.tsx
│   ├── pages/
│   │   ├── auth/                # Authentication pages
│   │   │   ├── Login.tsx
│   │   │   ├── SignUp.tsx
│   │   │   └── PasswordReset.tsx
│   │   ├── predict/             # Disease prediction pages
│   │   │   ├── Diabetes.tsx
│   │   │   ├── Heart.tsx
│   │   │   ├── Kidney.tsx
│   │   │   └── Cancer.tsx
│   │   ├── About.tsx
│   │   ├── Dashboard.tsx
│   │   ├── NotFound.tsx
│   │   ├── Profile.tsx
│   │   ├── Records.tsx
│   │   └── Research.tsx
│   ├── services/
│   │   ├── auth.ts              # Authentication service
│   │   └── prediction.ts        # AI prediction logic & record management
│   ├── store/
│   │   └── useAuthStore.ts      # Global auth & theme state (Zustand)
│   ├── types/
│   │   └── index.ts             # Shared TypeScript types
│   ├── App.css
│   ├── App.tsx                  # Root component & routing
│   ├── index.css
│   └── main.tsx                 # App entry point
├── index.html
├── package.json
├── tailwind.config.js
├── tsconfig.json
├── vite.config.ts
└── README.md
```

---

## ⚙️ Installation / Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or above recommended)
- npm (comes with Node.js)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Ai-Health-Detect-System.git
   cd Ai-Health-Detect-System-main
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open in browser**
   ```
   http://localhost:5173
   ```

5. **Build for production** *(optional)*
   ```bash
   npm run build
   ```

---

## 🚀 Usage

1. **Sign Up / Log In** — Create an account or log in to access the application.
2. **Navigate to a Prediction Page** — Choose from Diabetes, Heart, Kidney, or Cancer via the Sidebar.
3. **Enter Health Metrics** — Fill in the required clinical values (e.g., glucose level, BMI, cholesterol).
4. **Get Your Prediction** — Submit the form to receive an AI-generated risk score, confidence percentage, and risk classification (Low / Moderate / High).
5. **View Records** — All past predictions are automatically saved and accessible from the Records page.
6. **Explore Research** — Visit the Research page for disease-related health information and references.
7. **Manage Profile** — Update your personal details and toggle the app theme from the Profile page.

---

## 🖥️ Sample Output

After submitting health data on the Diabetes prediction page, a sample result looks like:

```
Disease   : Diabetes
Risk Score: 62%
Confidence: 87%
Result    : Moderate Risk

Details: Based on the submitted ailment info, risk is 62% and classified as Moderate.
```

The result is immediately saved to your personal Records history with a timestamp.

---

## 🔮 Future Improvements

- **Backend Integration** — Connect to a real ML model API (e.g., Flask/FastAPI with scikit-learn) for medically accurate predictions.
- **More Diseases** — Expand predictions to include liver disease, hypertension, stroke risk, and more.
- **Cloud Storage** — Replace localStorage with a cloud database (e.g., Firebase, Supabase) for cross-device access.
- **PDF Report Export** — Allow users to download their health prediction report as a PDF.
- **Doctor Referral System** — Suggest nearby specialists based on risk level and location.
- **Multilingual Support** — Add support for regional languages to improve accessibility.
- **Progressive Web App (PWA)** — Enable offline access and mobile app-like installation.
- **Advanced Analytics** — Show trend charts of risk scores over time on the Dashboard.

---

## 👤 Author

| Field | Details |
|---|---|
| **Name** | *(MONDI RATNA SAHITHI)* |
| **Role** | *(e.g., Full Stack Developer / Second Year Student)* |
| **LinkedIn** | [LinkedIn Profile](https://www.linkedin.com/in/mondi-ratna-sahithi-5219b232a?utm_source=share_via&utm_content=profile&utm_medium=member_android) |

---

> ⚠️ **Disclaimer:** This application is built for educational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider for medical decisions.
