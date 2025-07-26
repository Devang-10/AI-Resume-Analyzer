# AI Resume Analyzer

[![Vercel Deployment](https://img.shields.io/badge/Deployment-Vercel-black?style=for-the-badge&logo=vercel)](https://your-project-name.vercel.app)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

An intelligent web application that provides smart, actionable feedback on your resume using the power of AI. Built with React and the serverless Puter.js platform, this tool helps you optimize your resume for your dream job.

### [➡️ View Live Demo](https://your-project-name.vercel.app)

![AI Resume Analyzer Screenshot](https://i.imgur.com/vHqLd6f.png)

## ✨ Features

* **📄 Secure Resume Upload:** Upload your resume in PDF format directly from your device.
* **🧠 AI-Powered Analysis:** Leverages Anthropic's Claude 3.5 Sonnet via the Puter.js API to perform a deep analysis of your resume's content, structure, and phrasing.
* **🚀 Instant Feedback:** Receive constructive, point-by-point feedback in seconds.
* **💻 Modern & Responsive UI:** A clean, intuitive, and mobile-friendly interface built with React.
* **🌐 Serverless Architecture:** Runs entirely in the browser with no backend servers to manage, thanks to the Puter.js platform.

## 🛠️ Tech Stack

* **Frontend:** [React](https://react.dev/), [Vite](https://vitejs.dev/), [TypeScript](https://www.typescriptlang.org/)
* **Platform:** [Puter.js](https://puter.com/) for user authentication, file storage, and AI API calls.
* **AI Model:** Anthropic's Claude 3.7 Sonnet
* **Deployment:** [Vercel](https://vercel.com/)

## 🤔 How It Works

This project demonstrates the power of a fully serverless, "user-pays" application model using Puter.js.

1.  **Authentication:** The user authenticates using their Puter account. This grants the application secure, temporary access to the user's resources.
2.  **File Upload:** The resume is uploaded directly to the logged-in user's private Puter Drive.
3.  **API Call:** The frontend calls the `puter.ai.chat()` function, passing a reference to the uploaded file's path and a specific prompt for resume analysis.
4.  **Analysis:** The AI analysis is performed on behalf of the user, consuming *their* Puter account's AI credits.
5.  **Feedback:** The generated feedback is streamed back to the user's browser and displayed on the screen.

## 🚀 Getting Started

To run this project on your local machine, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd your-repo-name
    ```

3.  **Install dependencies:**
    ```bash
    npm install
    ```

4.  **Set up environment variables:**
    * Create a file named `.env` in the root of the project.
    * Add your Puter App's Client ID to it. You can find this in your app's settings on puter.com.
    ```
    VITE_PUTER_CLIENT_ID=your-puter-app-client-id
    ```

5.  **Run the development server:**
    ```bash
    npm run dev
    ```

6.  Open your browser and navigate to `http://localhost:5173`.

## 🚢 Deployment

This application is designed for easy deployment on [Vercel](https://vercel.com/).

1.  Import your Git repository into Vercel.
2.  Use the `Vite` framework preset.
3.  Verify the **Output Directory** is set to `dist`.
4.  **Crucially**, after your first deployment, you must add your Vercel URL (e.g., `https://your-project-name.vercel.app`) to the **Authorized Origins** list in your Puter App's settings to avoid CORS errors.

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---
_This project was created as a demonstration of building powerful, serverless AI applications with Puter.js._
