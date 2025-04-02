🚀 Swayam Course Automation Script

📌 Overview:

This Python script automates the login and course navigation process for Swayam, a government-run online learning platform. It uses Selenium WebDriver to:

✅ Log in via Microsoft

✅ Navigate to enrolled courses

✅ Detect available weeks

✅ Auto-fill assignment answers

✅ Submit assignments automatically

✨ Features

✔ Automated Login → Sign in to Swayam via Microsoft login using stored credentials.

✔ Course Selection → Automatically detects and opens your first enrolled course.

✔ Week Navigation → Lists available weeks and lets you select one.

✔ Assignment Handling → Detects and opens assignments for the selected week.

✔ Auto Submission → Automatically fills and submits assignment answers.

📂 Project Structure

📦 Swayam-Automation  
 ┣ 📜 .env  
 ┣ 📜 requirements.txt  
 ┣ 📜 app.py  
 ┗ 📜 README.md  

 
🛠️ Setup Instructions

1️⃣ Install Dependencies

Ensure you have Python 3.7+ installed, then install the required libraries:

pip install -r requirements.txt

Add the following dependencies to requirements.txt:

selenium  

python-dotenv  

2️⃣ Install Chrome WebDriver

Ensure Google Chrome is installed.

Download the Chrome WebDriver version matching your Chrome version:
👉 Download ChromeDriver

Place the WebDriver in a system PATH directory or specify its path in the script.

3️⃣ Setup Environment Variables

Create a .env file in the project directory and add your Swayam credentials:

SWAYAM_EMAIL=your-email@example.com  
SWAYAM_PASSWORD=yourpassword  

🚀 How to Run the Script
Run the script using:
python app.py

📜 Script Workflow
1️⃣ Launch Swayam My Courses Page

2️⃣ Login via Microsoft using stored credentials

3️⃣ Open the First Available Course

4️⃣ Detect Available Weeks and prompt the user to select one

5️⃣ Expand the Selected Week

6️⃣ Detect and Open Assignments

7️⃣ Prompt User for Answers

8️⃣ Auto-Fill the Assignment Answers

9️⃣ Submit the Assignment

🔧 Troubleshooting
Issue	Solution
selenium.common.exceptions.NoSuchElementException	The webpage structure might have changed. Update the XPath selectors in the script.
WebDriverException: chromedriver executable needs to be in PATH	Ensure ChromeDriver is correctly installed and in your system PATH.
Assignment answers not being filled	Verify the XPath for multiple-choice options and ensure correct indexing.
📌 Disclaimer:

This script is for educational purposes only. Automating interactions with online learning platforms may violate their terms of service. Use responsibly.

💡 Future Improvements:

✅ Support for multiple courses instead of just the first one.

✅ Auto-detect answers using AI/ML.

✅ Enhanced error handling and logging.

👨‍💻 Made with ❤️ by Krishnan. 🚀
