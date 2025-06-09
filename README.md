# 7speaking-bot-legacy
An attempt to automatize [7Speaking](7speaking.com). Works for "My7Speaking" and TOEIC (Trainings + Exams).

## How to install
- Install [Tampermonkey](https://www.tampermonkey.net/) for your browser.
- [Click here](https://github.com/Dixel1/7speaking-bot-legacy/raw/main/7speaking.user.js) to install the script or clic "RAW".
![image](https://github.com/Dixel1/7speaking-bot-legacy/assets/63664894/4d7af9cc-8765-4d2f-b4cc-52db5ff5f256)


- Go to [https://user.7speaking.com/home](https://user.7speaking.com/home) or [https://user.7speaking.com/workshop/exams-tests/toeic](https://user.7speaking.com/workshop/exams-tests/toeic) depending on what you want to complete (may not work properly on toeic mode. Please check https://github.com/Dixel1/7speaking-bot-legacy/issues).

## Edit the bot config :

![image](https://github.com/user-attachments/assets/0acc329c-1bf6-43e7-b908-fef4f1019f71)

### 1. ⚙️ Configure the probability of incorrect answers you want : ![image](https://github.com/user-attachments/assets/1ae47b69-c22d-4656-baa5-233aa249702b)

- ➡️ Put a number between **0.0** and **1.0** (Default error probability is **0.2 (20%)**). 

### 2. ⚙️ Configure the time spending parameter : ![image](https://github.com/user-attachments/assets/725c4389-10bf-4933-bbfb-e0598921d9bd)

- ➡️ **1** = The bot will wait **60-80%** of the real recommended time on the document before starting the Quizz.
- ➡️ **0** = The bot will start the Quizz **after 10s** spent on the document.

### 3. 💾 Save :

- **Ctrl + S** or :

![image](https://github.com/user-attachments/assets/c0c75cf0-4c7d-4a00-9306-3cd78af69be5)

### 4. 🔄 Refresh the 7speaking page !
  
- Let the bot **do its work**!
  
- Enjoy! 🎉

## Changelogs :

Here’s a summary of the changes made to the code:

### 1. **Metadata Block**:
  - Updated the script name to "7Speaking Bot Legacy - BETA" and incremented the version number from **8.7b1** to **8.7b2**. Added a @tuners field with the value "Astronas". Thanks to @Astronas for the hot features added to the bot.

### 2. **Anti-bot popup fix 🚫**:

- A fix for the **Anti-bot popup** that appeared with a suspicious activity message :

![image](https://github.com/user-attachments/assets/e203c431-6739-4963-af55-a3a3c3b1c69e)

- Thanks to the handlePopup function added by @astronas. This function catches the popup and automatically clicks **"Continue"** to allow the script to continue running 🔄.

### 3. **Random incorrect answers 🤔**:

- ![image](https://github.com/user-attachments/assets/1ae47b69-c22d-4656-baa5-233aa249702b)

- **🆕** A new feature that allows **generating random incorrect answers** to quiz questions with a user-defined probability has been added. This makes the responses more human-like and prevents perfect statistics 📊.

- You just have to modify **"errorProbability"** in the bot-script before use. Default error probability is **0.2 (20%)**.

### 4. **Realistic timing ⏰** :

- ![image](https://github.com/user-attachments/assets/725c4389-10bf-4933-bbfb-e0598921d9bd)

- **🆕** A timing function has been added. By setting the **useRealTime** variable to 1 at the beginning of the script, the script will retrieve the recommended duration from the current activity, minimize it by taking between **60% and 80%** of the value and wait for this time before moving on to the next activity ⏱️ :

- This makes the total time spent on a quiz and its initial document **more realistic** 📚. 

- Simply set this variable to **0** to disable this feature and allow activities to **run consecutively without delay** 🚀.

### 5. **Code comments 📝** :

- The code has been fully commented for better understanding 💡

### These updates aim to improve the script's compatibility and functionality, while enhancing its ability to simulate human behavior 🤖.
