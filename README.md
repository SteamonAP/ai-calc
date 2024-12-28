# AI-Powered Mathematical Image Calculator

## Overview
This project is an AI-powered tool that processes images containing mathematical expressions, equations, or graphical problems and solves them using advanced algorithms. It combines the power of FastAPI for backend processing and Vite + React for a seamless user interface.

## Features
- **Mathematical Expression Solver**: Processes images and evaluates expressions based on PEMDAS rules.
- **Equation Solver**: Handles simple equations and assigns values to variables.
- **Graphical Problem Analysis**: Detects and interprets visual mathematical problems.
- **Abstract Concept Detection**: Understands abstract ideas represented in images.

## Technologies Used
- **Backend**: FastAPI, Python, Pillow
- **Frontend**: React, TypeScript, Vite
- **Environment Management**: dotenv
- **Image Handling**: Base64 encoding/decoding

## Installation

### Prerequisites
- Node.js and npm
- Python 3.8+ and pip

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ai-math-image-calculator.git
   cd ai-math-image-calculator
Backend Setup

Navigate to the backend folder:
bash
Copy code
cd backend
Install Python dependencies:
bash
Copy code
pip install -r requirements.txt
Add environment variables in .env:
env
Copy code
GEMINI_API_KEY=your_api_key_here
Start the backend server:
bash
Copy code
python main.py
Frontend Setup

Navigate to the frontend folder:
bash
Copy code
cd frontend
Install dependencies:
bash
Copy code
npm install
Start the development server:
bash
Copy code
npm run dev
Access the application in your browser:

arduino
Copy code
http://localhost:3000
API Endpoints
POST /calculate
Input: Base64-encoded image and user-defined variables.
Output: Calculated results based on the provided image.



# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

- Replace `tseslint.configs.recommended` to `tseslint.configs.recommendedTypeChecked` or `tseslint.configs.strictTypeChecked`
- Optionally add `...tseslint.configs.stylisticTypeChecked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and update the config:

```js
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  // Set the react version
  settings: { react: { version: '18.3' } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs['jsx-runtime'].rules,
  },
})
```
