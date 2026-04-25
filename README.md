# QuickAI 🚀

**QuickAI** is an all-in-one AI productivity and creative suite designed to streamline your workflow. From generating high-quality articles and catchy blog titles to advanced image manipulation and professional resume reviews, QuickAI leverages state-of-the-art AI models to provide a premium user experience.

![QuickAI Banner](https://img.shields.io/badge/AI-Productivity-blue?style=for-the-badge)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

---

## ✨ Key Features

### 📝 AI Writing Suite
- **Article Generator**: Create long-form, SEO-friendly articles in seconds using **Llama 3.1** (via Groq).
- **Blog Title Generator**: Generate engaging and viral-ready titles for your content.

### 🖼️ AI Image Tools
- **Text-to-Image**: Transform your ideas into stunning visuals using the **ClipDrop API**.
- **Background Removal**: Effortlessly remove backgrounds from any image with high precision.
- **Generative Object Removal**: Remove unwanted objects from your photos using AI-powered "in-painting" techniques.

### 📄 Professional Resume Reviewer
- Upload your resume in **PDF format** and receive constructive feedback, identifying strengths and areas for improvement.

### 💳 Premium Ecosystem
- **Tiered Access**: Free and Premium plans managed via **Clerk** metadata.
- **Usage Tracking**: Real-time tracking of AI generations.
- **Persistent History**: All your creations are securely stored and accessible anytime.

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: React 19 + Vite
- **Styling**: Tailwind CSS 4
- **Authentication**: Clerk (clerk-react)
- **Routing**: React Router 7
- **Icons**: Lucide React
- **Notifications**: React Hot Toast

### Backend
- **Runtime**: Node.js
- **Framework**: Express 5
- **Database**: Neon (Serverless PostgreSQL)
- **AI Models**: Groq (Llama 3.1 8B), ClipDrop API
- **Storage**: Cloudinary (Image hosting & transformations)
- **File Handling**: Multer & PDF-Parse

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- A [Clerk](https://clerk.com/) account
- A [Neon DB](https://neon.tech/) account
- A [Groq Cloud](https://console.groq.com/) account
- A [Cloudinary](https://cloudinary.com/) account
- A [ClipDrop](https://clipdrop.co/apis) API key

### 1. Clone the repository
```bash
git clone https://github.com/your-username/QuickAI.git
cd QuickAI
```

### 2. Backend Setup
```bash
cd server
npm install
```
Create a `.env` file in the `server` directory and add the following:
```env
CLERK_PUBLISHABLE_KEY=your_clerk_pub_key
CLERK_SECRET_KEY=your_clerk_secret_key
DATABASE_URL=your_neon_db_url
GROQ_API_KEY=your_groq_api_key
CLIPDROP_API_KEY=your_clipdrop_api_key
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```
Start the server:
```bash
npm run dev
```

### 3. Frontend Setup
```bash
cd ../client
npm install
```
Create a `.env` file in the `client` directory:
```env
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_pub_key
VITE_SERVER_URL=http://localhost:5000
```
Start the client:
```bash
npm run dev
```

---

## 📂 Project Structure

```text
QuickAI/
├── client/           # React + Vite frontend
│   ├── src/          # Components, Hooks, Context, Pages
│   └── public/       # Static assets
├── server/           # Express backend
│   ├── configs/      # DB, Cloudinary, Multer configurations
│   ├── controllers/  # Route logic
│   ├── routes/       # API endpoints
│   └── middlewares/  # Auth & usage limits
└── README.md         # Documentation
```

---

## 📜 License
This project is licensed under the ISC License.

---

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

---

**Built with ❤️ for the AI community.**
