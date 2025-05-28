# 7speaking-bot-legacy
An attempt to automatize [7Speaking](7speaking.com). Works for "My7Speaking" and TOEIC (Trainings + Exams).

## How to install
- Install [Tampermonkey](https://www.tampermonkey.net/) for your browser.
- [Click here](https://github.com/Dixel1/7speaking-bot-legacy/raw/main/7speaking.user.js) to install the script or clic "RAW".
![image](https://github.com/Dixel1/7speaking-bot-legacy/assets/63664894/4d7af9cc-8765-4d2f-b4cc-52db5ff5f256)


![image](https://github.com/user-attachments/assets/e203c431-6739-4963-af55-a3a3c3b1c69e)

![image](https://github.com/user-attachments/assets/a163702d-0de9-4eb4-a6a2-74893e0516ea)


- Go to [https://user.7speaking.com/home](https://user.7speaking.com/home) or [https://user.7speaking.com/workshop/exams-tests/toeic](https://user.7speaking.com/workshop/exams-tests/toeic) depending on what you want to complete (may not work properly on toeic mode. Please check https://github.com/Dixel1/7speaking-bot-legacy/issues).
- Let the bot do its work.
- Enjoy!

## Changelogs :

Here’s a summary of the changes made to the code:

1. Metadata Block:
  - Updated the script name to "7Speaking Bot Legacy - BETA" and incremented the version number from 8.5 to 8.7b2. Added a @tuners field with the value "Astronas".
These updates reflect the new **working** beta version thanks to @juliendnte. Thanks to @astronas for the hot features added to the bot.

2. Anti-bot popup fix 🚫:
- A fix for the Anti-bot popup that appeared with a suspicious activity message, thanks to the handlePopup function added by @astronas. This function catches the popup and automatically clicks "Continue" to allow the script to continue running 🔄.

3. Random incorrect answers 🤔:
- A new feature that allows generating random incorrect answers to quiz questions with a user-defined probability. This makes the responses more human-like and prevents perfect statistics 📊.

- You just have to modify "errorProbability" in the bot-script before use. Default error probability : 0.2 (20%).

4. Realistic timing ⏰ :
- A timing function has been added. By setting the **useRealTime** variable to 1 at the beginning of the script, the script will retrieve the recommended duration for the current activity, minimize it between **60% and 80%**, and wait for this time before moving on to the next activity ⏱️. This makes the total time spent on a quiz and its initial document more realistic 📚. Simply set this variable to 0 to disable this feature and allow activities to run consecutively without delay 🚀.

5. Code comments 📝 :
- The code has been fully commented for better understanding 💡

These updates aim to improve the script's compatibility and functionality, while enhancing its ability to simulate human behavior 🤖.
