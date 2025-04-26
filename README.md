## Smart Email Generator
A full-stack AI-powered Smart Email Generator that uses Java Spring Boot for the backend, React for the frontend, and Google Gemini API to automatically generate intelligent email replies. The project also includes a Chrome Extension for seamless integration with Gmail.

🚀 Features
✉️ Generate smart, context-aware email replies with Google Gemini
🧠 AI-powered natural language understanding
🌐 Full-stack web app (Java Spring Boot + React)
🧩 Chrome Extension for Gmail integration
🔐 Secure API integration
⚡ Fast and responsive UI

## Project Structure
smart-email-generator/ │ ├── backend/ # Java Spring Boot backend │ └── src/ │ └── main/java/com/example/email/ │ ├── frontend/ # React frontend │ └── src/ │ └── components/ │ ├── chrome-extension/ # Chrome extension source │ └── manifest.json │ └── content.js │ └── popup.html │ └── README.md

## Tech Stack
Layer	Tech
- Backend	Java, Spring Boot, REST API
- Frontend	React, JavaScript, MaterialUI
- AI Engine	Google Gemini API
- Extension	Chrome Extension (Manifest v3)
- Setup Instructions
- Backend (Spring Boot)
- cd backend
- ./mvnw spring-boot:run

Make sure to configure your Google Gemini API Key in application.properties:
gemini.api.key=your_google_gemini_api_key

## Frontend (React)
- cd frontend
- npm install
- npm start
- Update your .env to point to your backend: REACT_APP_API_URL=http://localhost:8080

## Chrome Extension
- Go to chrome://extensions/ Enable Developer Mode Click Load unpacked Select the chrome-extension/ folder Start using it in Gmail

## How It Works
- User selects an email to reply to. Chrome Extension extracts email content and sends it to backend. Backend processes content and sends request to Google Gemini. Gemini returns a smart reply. The response is shown in the Chrome Extension popup for user review and editing.

## API Endpoints
- Method   - Endpoint         - Description

POST       - /api/generate  - Generates a smart reply using Gemini

Example Request: { "emailContent": "Hi, can you send me the report by tomorrow?" }

## Environment Variables
Set the following in your .env or application.properties:

- GEMINI_API_KEY

- REACT_APP_API_URL

## Future Improvements
- Conversation thread support

- User authentication (OAuth)

- Multilingual support

- Mobile support

## Authors
Afrid Pathan

🌟 Show Your Support If you like this project, give it a ⭐ on GitHub or share it!
