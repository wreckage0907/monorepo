# Monorepo Template

This repository serves as a template for a monorepo setup that includes both backend and frontend projects. The backend is pre-configured with a **FastAPI** setup, and the frontend can be built using either **Flutter** or **Next.js**, or any other framework you prefer.

## Backend (FastAPI)

### 1. Prerequisites
Make sure you have the following installed:
- Python 3.8+
- pip (Python package installer)
- Virtual environment tool (optional but recommended)

### 2. Setup Instructions
1. Navigate to the `backend/` directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows use: env\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the FastAPI server:
   ```bash
   uvicorn main:app --reload
   ```

5. The backend will be running on `http://127.0.0.1:8000`. You can view the automatic documentation provided by FastAPI at `http://127.0.0.1:8000/docs` or `http://127.0.0.1:8000/redoc`.

---

## Frontend (Flutter Setup)

### 1. Prerequisites
Make sure you have the following installed:
- [Flutter](https://flutter.dev/docs/get-started/install) (Stable channel)
- A text editor like VSCode or Android Studio

### 2. Setup Instructions
1. Navigate to the `frontend/` directory:
   ```bash
   cd frontend
   ```

2. Create a new Flutter project (if none exists yet):
   ```bash
   flutter create .
   ```

3. Open the project in your editor and start developing your Flutter app.

4. To run the Flutter app:
   - On a physical or virtual device, run:
     ```bash
     flutter run
     ```

5. Make sure your backend (FastAPI) is running for API calls if your Flutter app interacts with the backend.

---

## Frontend (Next.js Setup)

### 1. Prerequisites
Make sure you have the following installed:
- Node.js (v14 or higher)
- npm or yarn

### 2. Setup Instructions
1. Navigate to the `frontend/` directory:
   ```bash
   cd frontend
   ```

2. Create a new Next.js project:
   ```bash
   npx create-next-app@latest .
   ```

3. Follow the prompts to set up the Next.js project.

4. To start the development server:
   ```bash
   npm run dev
   ```
   The Next.js app will be running at `http://localhost:3000`.

5. You can start developing your Next.js frontend and use the FastAPI backend for any API interactions.

---

## Running the Projects

### Backend (FastAPI)
1. Navigate to the `backend/` folder and run:
   ```bash
   uvicorn main:app --reload
   ```

### Frontend (Flutter)
1. Navigate to the `frontend/` folder and run:
   ```bash
   flutter run
   ```

### Frontend (Next.js)
1. Navigate to the `frontend/` folder and run:
   ```bash
   npm run dev
   ```

---

This README provides the necessary steps to set up and start using the monorepo template for both the FastAPI backend and the Flutter or Next.js frontend development.
