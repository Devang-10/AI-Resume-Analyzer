# AI Resume Analyzer

An intelligent web application that provides smart, actionable feedback on your resume using the power of AI. Built with React and the serverless Puter.js platform, this tool helps you optimize your resume for your dream job.

### View Live Demo ➡️ [(Resumind - AI Mind for you Resume)](https://ai-resume-analyzer-kappa-two.vercel.app)

## Screenshots

<span>
    <img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/8abe35d8-b714-4f19-ad29-724faf1e965d" />
</span>
<span>
    <img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/cb78532c-12ee-4006-91ac-fcc6b55a684e" />
</span>
<span>
    <img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/fc549921-dce0-415f-8c2c-8341999e2e48" />
</span>
<span>
    <img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d32a28cf-b65b-4bcb-a502-9cf4d8916d8a" />
</span>

## ✨ Features

* **📄 Secure Resume Upload:** Upload your resume in PDF format directly from your device.
* **🧠 AI-Powered Analysis:** Leverages Anthropic's Claude 3.7 Sonnet via the Puter.js API to perform a deep analysis of your resume's content, structure, and phrasing.
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

---
_This project was created as a demonstration of building powerful, serverless AI applications with Puter.js._
