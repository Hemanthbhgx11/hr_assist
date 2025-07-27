Virtual HR Interview Assistant (Cyberpunk Theme)
This is a client-side web application designed to assist HR professionals and hiring managers in generating relevant interview questions based on job requirements and applicant resumes. The tool leverages the Google Gemini API to intelligently formulate questions that aim to reveal an applicant's readiness, problem-solving skills, and specific experiences relevant to a given role. It features a sleek cyberpunk-inspired user interface.

Features
AI-Powered Question Generation: Uses the Gemini API to create tailored interview questions.

Job Requirements Input: Allows users to paste job descriptions or key requirements.

Applicant Resume Input: Supports pasting key details from an applicant's resume for personalized questions.

Cyberpunk Theme: A visually distinct dark theme with reddish-blue gradients and neon accents.

Responsive Design: Adapts to various screen sizes for usability on desktop and mobile devices.

Direct LinkedIn Link: Includes a clickable link to the developer's LinkedIn profile.

Important Notes
No Direct File Parsing: Due to browser security limitations, this client-side application does not support direct file uploads (e.g., PDF, DOCX) for resume analysis. Users must copy and paste the relevant text content from resumes into the designated input field.

No Email/LinkedIn Automation: This tool focuses solely on question generation. Direct integration with email services (for sending/receiving emails) or social media platforms (like LinkedIn for automated messaging) is beyond the scope of a client-side web application due to security, privacy, and API access limitations. Such functionalities would require robust backend systems and explicit third-party API permissions.

API Key Security (Crucial for Deployment):

This application uses the Google Gemini API. The provided code explicitly includes the API key (AIzaSyAyn6G2nP83vzlHQZ8vzjzsiVrker1sBYU).

For production environments, directly embedding API keys in client-side code is NOT recommended. This exposes your key to anyone who views the page source.

Secure Alternative: For a production-ready solution, it is highly recommended to use a backend server (e.g., Firebase Cloud Functions, Node.js, Python Flask) to proxy your API requests. The backend would securely store your API key as an environment variable and make the actual calls to the Gemini API, returning the results to your client-side application.

Getting Started
To run this application, you only need a web browser.

Local Setup
Save the Code: Save the provided HTML code (from the Canvas document) as index.html on your computer.

Open in Browser: Open the index.html file in your preferred web browser.

Deployment (for wider access)
Since this is a static HTML file, you can deploy it easily using various static site hosting services.

Obtain a Gemini API Key (if deploying outside Canvas):

Go to Google AI Studio.

Log in with your Google account.

Follow the prompts to create a new API key.

Important: The current code already has the API key AIzaSyAyn6G2nP83vzlHQZ8vzjzsiVrker1sBYU embedded. If you generate a new key for your own deployment, you would replace this value in the index.html file:

const apiKey = "YOUR_NEWLY_GENERATED_API_KEY_HERE";

Remember the security warning above about exposing API keys in client-side code.

Choose a Hosting Platform:

GitHub Pages: Upload index.html to a public GitHub repository, then enable GitHub Pages in your repository settings.

Netlify / Vercel: Connect your GitHub repository to these services for easy, continuous deployment.

Firebase Hosting: A robust option for hosting web applications, especially if you plan to integrate other Firebase services (like Cloud Functions for secure API key handling).

Usage
Open the application in your web browser.

In the "Job Requirements" text area, paste the job description or key skills required for the role.

In the "Applicant Resume (Paste Key Details)" text area, copy and paste relevant sections from the applicant's resume.

Click the "Generate Interview Questions" button.

The generated interview questions will appear in the "Generated Interview Questions" section below.

Built By
Hemanth Goud Burra
