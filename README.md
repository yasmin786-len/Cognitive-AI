# 🧠 CognitiveNotes – AI-Powered Notes Application

CognitiveNotes is a full-stack AI-powered note-taking application designed to help users create, organize, manage, and access their notes efficiently. It aims to improve productivity through AI-powered summaries and smart note organization.

## 🚀 Features

- **User Authentication:** Secure user registration and login using JWT authentication.
- **Note Management:** Create, view, and manage personal notes.
- **AI-Powered Summaries:** Generate summaries of notes using the Groq API.
- **Smart Categorization:** Organize notes for easier access.
- **Secure Access:** Protect user-specific resources through authentication.
- **Responsive Interface:** User-friendly React-based frontend.

## 🛠️ Tech Stack

### Frontend
- React.js
- Vite
- JavaScript
- HTML5
- CSS3
- Axios

### Backend
- Java 21
- Spring Boot 3
- Spring Security
- Spring Data JPA
- JWT Authentication
- Maven

### Database
- PostgreSQL

### AI Integration
- Groq API

### Development Tools
- Git and GitHub
- IntelliJ IDEA / VS Code
- Postman
- Ubuntu / Linux

## 📁 Project Structure

The project is organized into separate frontend and backend applications.

```text
CognitiveNotes/
│
├── CognativeNotes/              # Spring Boot Backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   └── resources/
│   │   └── test/
│   ├── pom.xml
│   └── mvnw
│
└── CognativeNotes-Frontend/     # React Frontend
    ├── public/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   └── services/
    ├── package.json
    └── vite.config.js
```

## ⚙️ Installation and Setup

### Prerequisites

Install the following before running the application:

- Java 21 or later
- Node.js and npm
- PostgreSQL
- Git
- Groq API key

### 1. Clone the repositories

Clone the backend and frontend repositories separately:

```bash
git clone YOUR_BACKEND_REPOSITORY_URL
git clone YOUR_FRONTEND_REPOSITORY_URL
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd CognativeNotes
```

Configure your environment variables:

```bash
export DB_URL="jdbc:postgresql://localhost:5432/cognativenotes_db"
export DB_USERNAME="your_postgres_username"
export DB_PASSWORD="your_postgres_password"
export GROQ_API_KEY="your_groq_api_key"
export JWT_SECRET="your_jwt_secret"
```

Make sure the PostgreSQL database exists before starting the application.

Run the backend:

```bash
chmod +x mvnw
./mvnw spring-boot:run
```

Backend URL:

```text
http://localhost:8084
```

### 3. Frontend Setup

Open another terminal and navigate to the frontend directory:

```bash
cd CognativeNotes-Frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the local URL displayed in your terminal, usually:

```text
http://localhost:5170
```

## 🔗 Application Configuration

The frontend communicates with the backend through Axios.

Development API base URL:

```text
http://localhost:8084/api
```

Ensure the frontend API configuration matches the backend port.

## 🔐 Environment Variables

| Variable | Description |
|---|---|
| `DB_URL` | PostgreSQL database connection URL |
| `DB_USERNAME` | PostgreSQL username |
| `DB_PASSWORD` | PostgreSQL password |
| `GROQ_API_KEY` | Groq API key |
| `JWT_SECRET` | Secret used for JWT signing |

**Security Note:** Never commit API keys, database passwords, JWT secrets, or other sensitive credentials to GitHub. Use environment variables and keep `.env` files out of version control.

## 🧪 Testing

- Test backend APIs using Postman.
- Test registration and login functionality.
- Verify JWT-protected endpoints.
- Test note creation and retrieval.
- Verify AI integration and summary generation.

## 🎯 Project Objective

The main objective of CognitiveNotes is to make note-taking smarter and more productive by combining full-stack web development, secure authentication, database management, and AI integration.

## 🔮 Future Enhancements

- Voice-to-text note creation.
- Advanced AI-based note summarization.
- Semantic search across notes.
- Note sharing and collaboration.
- Export notes as PDF.
- Mobile-friendly experience.

## 👩‍💻 Author

Sayyad Yasmin
