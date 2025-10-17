LightUpDiwali – The Ultimate Diwali Wishing Experience 🪔
Welcome to LightUpDiwali, a beautifully interactive web application designed to celebrate the festival of lights. This project allows users to embark on a festive journey: lighting diyas, decorating a virtual home, launching spectacular fireworks, and generating a personalized, AI-powered Diwali wish to share with friends and family.
✨ [Live Demo Link Here] ✨
🌟 Features
Interactive Welcome: Begin the journey by lighting a virtual diya with a beautiful glow animation.
Drag-and-Drop Decoration: Get creative by decorating a traditional Indian house with diyas, lanterns, rangoli, and string lights.
Dynamic Fireworks: Light up the night sky by clicking to launch stunning, realistic fireworks, each bursting with a festive message.
AI-Powered Wish Generation: Using the power of the Google Gemini API, generate unique and heartfelt Diwali wishes.
Personalized for You: The experience is automatically personalized from "Shah Dhruv" to any recipient.
Shareable Greeting Card: The final wish is presented as a beautiful digital greeting card.
Multiple Sharing Options:
Generate a unique shareable link.
Share directly to WhatsApp.
Download the greeting card as a PNG image.
Ambient Experience: Enjoy festive background music with an easy-to-use mute/unmute control.
Responsive Design: A seamless experience across desktops, tablets, and mobile devices.
🚀 Tech Stack
This project is built with a modern and powerful set of technologies:
Frontend: React.js & TypeScript
AI Model: Google Gemini API (gemini-2.5-flash)
Styling: Tailwind CSS for rapid, utility-first styling.
Fonts: Google Fonts (Poppins and Dancing Script) for beautiful typography.
Card Download: html2canvas to convert the final greeting card from HTML to a downloadable PNG image.
Animations: Pure CSS keyframe animations for glowing effects and realistic fireworks.
📁 Project Structure
The codebase is organized into logical modules for maintainability and scalability.
code
Code
/
├── public/
│   └── (Static assets like favicon)
├── src/
│   ├── components/
│   │   ├── WelcomePage.tsx
│   │   ├── DecorationPage.tsx
│   │   ├── FireworksPage.tsx
│   │   ├── WishCreatorPage.tsx
│   │   ├── SharePage.tsx
│   │   └── Icons.tsx
│   ├── services/
│   │   └── geminiService.ts   # Handles all Google Gemini API calls
│   ├── App.tsx                # Main component, manages scenes and state
│   ├── index.tsx              # React entry point
│   ├── types.ts               # TypeScript type definitions
│   └── constants.ts           # Application-wide constants
├── index.html                 # Main HTML file
└── ... (config files)
⚙️ Getting Started
To run this project locally, follow these simple steps.
Prerequisites
Node.js (v18 or later)
A package manager like npm or yarn
A Google Gemini API Key. You can get one from Google AI Studio.
Installation & Setup
Clone the repository:
code
Bash
git clone https://github.com/your-username/light-up-diwali.git
cd light-up-diwali
Install dependencies:
code
Bash
npm install
Set up your environment variables:
Create a file named .env in the root of your project and add your Google Gemini API key:
code
Code
# .env
API_KEY=YOUR_GEMINI_API_KEY
Note: The app is configured to use process.env.API_KEY to access this value.
Run the development server:
code
Bash
npm run start
The application should now be running on http://localhost:3000.
🪔 The User Journey
Welcome: The user is greeted with a single unlit diya. Clicking it ignites the flame and transitions to the next scene.
Decorate: The user can drag and drop festive items onto a house illustration. Once at least one item is placed, a button appears to continue.
Fireworks: The scene transitions to a night sky. The user can click anywhere to launch beautiful fireworks. After a few clicks, a button to create a wish appears.
Create Wish: The user enters the recipient's name. The app then calls the Gemini API to generate a unique wish.
Share: A final, beautifully designed greeting card is displayed with the recipient's name, the sender's name ("Shah Dhruv"), and the AI-generated message. From here, the user can copy a link, share on WhatsApp, or download the card as an image.
✍️ Author
Shah Dhruv
