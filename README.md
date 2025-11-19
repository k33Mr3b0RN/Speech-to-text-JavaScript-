🎙️ Real-Time Mobile Speech-to-Text Transcriber
This is a simple, single-file web application that leverages the Web Speech API to provide real-time, high-accuracy voice transcription directly within your web browser.
It is designed to be fully responsive and works optimally on mobile devices, making it a perfect tool for quickly dictating notes or transcribing short pieces of audio.
✨ Features
 * Real-Time Transcription: See your words appear as you speak (interim results are shown in gray italics).
 * Final Confirmation: Confirmed text is finalized and added to the transcript (shown in black).
 * Copy Functionality: A dedicated button allows you to copy the entire transcribed text to your clipboard instantly.
 * Mobile-First Design: A clean, responsive interface using modern Tailwind CSS ensures an excellent experience on any screen size.
🚀 How to Use & Run
Since this application uses the browser's built-in microphone access, it has a strict security requirement. It will NOT work reliably when opened directly from your file system (file:///).
The browser must recognize the source as secure, which means running it over http://localhost or, preferably, https://.
1. Recommended Method (HTTPS Hosting)
This is the only way to guarantee the app works correctly on mobile devices (iOS/Android):
 * Host the file: Upload the single file, speech_to_text.html, to a free static hosting service like:
   * GitHub Pages (Requires a GitHub repo)
   * Vercel
   * Netlify
 * Access the Secure Link: Open the generated https:// link on your desktop or mobile phone.
 * Grant Permission: Click the microphone button and grant the browser permission to access your microphone when prompted.
2. Local Testing Method (For Desktop Only)
If you are just testing on a desktop computer, you can use a simple local server:
 * Install HTTP Server: Ensure you have Node.js installed, then install the server:
   npm install -g http-server

 * Start the Server: Navigate to the directory where you saved speech_to_text.html and run:
   http-server

 * Open: Access the application using the local address provided (e.g., http://localhost:8080/speech_to_text.html).
💻 Technologies Used
 * HTML5: Structure of the single-page application.
 * JavaScript (Vanilla): Implements the logic for the Web Speech API, handling microphone input, transcription, and text output.
 * Web Speech API: The core browser feature used for speech recognition.
 * Tailwind CSS: Provides utility classes for modern, responsive styling.
 * Lucide Icons: Used for the clean, vector-based microphone and copy icons.
📄 License
This project is open-sourced under the MIT License.
