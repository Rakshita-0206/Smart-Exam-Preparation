# 🎯 Smart Exam Preparation Platform

> An AI-powered competitive exam preparation platform that delivers intelligent topic selection, personalized study resources, and a fully responsive user experience — built with modern web technologies and the Gemini API.

[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat&logo=react)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat&logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-3-06B6D4?style=flat&logo=tailwindcss)](https://tailwindcss.com/)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=flat&logo=vite)](https://vitejs.dev/)
[![Gemini API](https://img.shields.io/badge/Gemini-API-4285F4?style=flat&logo=google)](https://ai.google.dev/)
[![Deployed on Vercel](https://img.shields.io/badge/Deployed-Vercel-000000?style=flat&logo=vercel)](https://vercel.com/)

---

## 🌐 Live Demo

🔗 **[View Live Application →](https://github.com/Rakshita-0206/Smart-Exam-Preparation)**

---

## 📌 Project Overview

Smart Exam Preparation is a full-stack, AI-integrated web application designed to streamline how students prepare for competitive exams. By leveraging Google's Gemini API, the platform provides dynamically generated, contextual study content, making exam prep smarter and more efficient.

This project demonstrates practical application of **AI API integration**, **component-based architecture**, and **responsive UI design** — skills directly applicable to real-world product and software engineering roles.

---

## ✨ Key Features

- **AI-Powered Topic Selection** — Uses the Gemini API to intelligently suggest and prioritize study topics based on user input and exam patterns.
- **Personalized Study Resources** — Dynamically generates study material, summaries, and practice questions tailored to each user.
- **Responsive UI** — Fully mobile-friendly interface built with Tailwind CSS for a polished cross-device experience.
- **Modern Developer Tooling** — Built with Vite for blazing-fast builds and hot module replacement during development.
- **Type-Safe Codebase** — End-to-end TypeScript implementation for maintainability and reduced runtime errors.
- **Production Deployment** — Deployed on Vercel with CI/CD integration via GitHub.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend Framework | React 18 |
| Language | TypeScript |
| Styling | Tailwind CSS |
| Build Tool | Vite |
| AI Integration | Google Gemini API |
| Deployment | Vercel + GitHub Pages |
| Config/Env | `.env` based environment variable management |

---

## 🚀 Getting Started

### Prerequisites

- Node.js v18+
- npm or yarn
- A valid [Gemini API key](https://ai.google.dev/)

### Installation

```bash
# Clone the repository
git clone https://github.com/Rakshita-0206/Smart-Exam-Preparation.git
cd Smart-Exam-Preparation

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Add your Gemini API key to .env

# Start the development server
npm run dev
```

The app will be available at `http://localhost:5173`.

### Build for Production

```bash
npm run build
```

---

## 📁 Project Structure

```
Smart-Exam-Preparation/
├── index.html              # App entry point
├── index.js                # Root JS entry
├── src/                    # Source files
│   ├── components/         # Reusable React components
│   ├── pages/              # Route-level page components
│   ├── services/           # Gemini API integration layer
│   └── types/              # TypeScript type definitions
├── public/                 # Static assets
├── .env.example            # Environment variable template
├── tailwind.config.js      # Tailwind CSS configuration
├── vite.config.js          # Vite build configuration
├── postcss.config.js       # PostCSS configuration
└── vercel.json             # Vercel deployment config
```

---

## 🤖 AI Integration Details

This project integrates with the **Google Gemini API** to power core features:

- **Dynamic Content Generation** — Exam-specific study notes and topic explanations are generated on-demand using Gemini's language capabilities.
- **Intelligent Recommendations** — The app sends structured prompts to the Gemini API to recommend what to study next based on exam type and progress.
- **Abstracted API Layer** — All API calls are encapsulated in a dedicated `services/` module, keeping components clean and the integration easily swappable.

> API keys are managed securely via environment variables and are never exposed to the client bundle.

---

## 🧠 What I Learned / Technical Highlights

- Designed and implemented a **production-ready AI integration** using REST API calls to the Gemini endpoint with proper error handling and loading states.
- Built a **fully typed React application** using TypeScript interfaces and generics, ensuring type safety across components and API responses.
- Applied **Tailwind CSS utility-first patterns** to build a responsive, accessible UI without writing custom CSS.
- Configured **Vite** for optimized production builds and fast local development cycles.
- Managed deployment pipelines using **Vercel**, including environment variable configuration for production secrets.

---

## 🔧 Environment Variables

Create a `.env` file based on `.env.example`:

```env
VITE_GEMINI_API_KEY=your_gemini_api_key_here
```

> Never commit your `.env` file. It is listed in `.gitignore`.

---

## 📦 Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start local development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview the production build locally |

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👩‍💻 Author

**Rakshita**
- GitHub: [@Rakshita-0206](https://github.com/Rakshita-0206)

---

> ⭐ If you find this project useful or interesting, consider giving it a star on GitHub!
