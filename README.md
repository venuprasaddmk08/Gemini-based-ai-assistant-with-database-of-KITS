1. KITS-VOICE_ASSISTANT
2. Unclear details of machines and PCs in KITS
3. ai that had information about the ps adn machines in KITS
4. Answers general questions as well as information about equipment in KITS
5. RasberryPI, Mic, Speaker
6. Software Requirements: Python 3.x, SpeechRecognition, pyttsx3, OpenPyXL, Google Gemini API, ALSA/arecord, Linux OS, Git, and GitHub
7. Technology Used: Python, Google Gemini AI, Speech Recognition, Text-to-Speech (pyttsx3), Excel-based Knowledge Base (OpenPyXL), and Linux/ALSA Audio
8. System Architecture: User Voice Input → Microphone & Speech Recognition → Database Search → Excel Knowledge Base → Google Gemini AI → AI-Generated Response → Text-to-Speech → User.
9. Database Structure: The system uses an Excel-based knowledge base consisting of a main database.xlsx file and multiple machine-specific .xlsx files stored in the Karunya_Machine_Knowledge_Base_Excel folder. Each worksheet uses the first row as field headers, while subsequent rows contain records; source file and sheet information are also tracked internally
10. git clone https://github.com/venuprasaddmk08/Gemini-based-ai-assistant-with-database-of-KITS.git
    cd Gemini-based-ai-assistant-with-database-of-KITS
    pip install -r requirements.txt
11. export GEMINI_API_KEY="YOUR_GEMINI_API_KEY"
12. python main.py
13. Sample Questions
    ~ What computers are available in the KITS lab?
    ~How many PCs do we have?
    ~What are the specifications of PC 1?
    ~What processor does PC 5 have?
    ~What is the RAM capacity of PC 10?
    ~What operating system is installed on PC 3?
    ~Which machines are available in the studio?
    ~What are the specifications of a particular machine?
    ~Tell me about the equipment available in the lab.
    ~What information do you have about PC 2?
14. Project Limitations
    >Requires an active Gemini API key and internet connection for AI responses.
    >Currently designed primarily for Linux, as it uses the arecord command for audio recording.
    >Voice recognition depends on the availability and quality of the microphone and speech-recognition service.
    >The assistant can only provide equipment information available in the Excel knowledge base and should not invent missing specifications.
    >Changes to the Excel database require restarting the application to reload the data.
    >The system currently uses a keyword-based database search, which may not always identify the most relevant records for complex questions.
15. <a href="https://github.com/venuprasaddmk08/Gemini-based-ai-assistant-with-database-of-KITS" target="_blank">
  <img src="https://img.shields.io/badge/View%20Source%20Code-GitHub-black?style=for-the-badge&logo=github" alt="View Source Code">
</a>
