# !Toohak - a free kahoot clone

## Installation Guide

1. install the latest LTS node version (current version as of initialization is **20.11.0**; use [nvm](https://github.com/nvm-sh/nvm) to install it)
2. run `cd toohak-be && npm install` to install all the project dependencies
3. run `cd toohak-fe && npm install` to install all the project dependencies
4. in `toohak-be`, create a `.env` file with the following value:
   - `MONGO_URI=mongodb+srv://toohak_team:krucR4F8uzbFmaWI@toohak.jzfjdxn.mongodb.net/?retryWrites=true&w=majority`
5. in `toohak-fe`, create a `.env` file with the following values:
   - `VITE_WEBSOCKET_URL=http://localhost:3000/`
   - `VITE_BACKEND_URL=http://localhost:3000`
6. in a seperate terminal window, run `cd toohak-be && npm run dev`
7. in a seperate terminal window, run `cd toohak-fe && npm run dev`
8. navigate to http://localhost:5173/ to use !toohak

## User Guide

### Build Quiz

1. in a browser tab (host tab), navigate to http://localhost:5173/ and press **Build Quiz**
2. in the text field that contains "Untitled Quiz," replace the text with the desired quiz name
3. in the "Question" text field, enter your question
4. in the "Type" dropdown menu, select your question type (multiple choice or true/false)
5. if the question is **multiple choice**, fill out the answer text fields with the possible answer choices
6. in the "Correct Answer" dropdown menu, select the answer you want to be considered as correct
7. press the button with the '+' to create a new question or the button with the trash can to delete the question from the quiz
8. repeat steps 3-6 until satisfied with the number of questions
9. press **Publish Quiz** to finish building your quiz

### Play Quiz

1. in a browser tab (host tab), navigate to http://localhost:5173/ and press **Play**
2. to create a room for players to join, press **Create Room**
3. in another browser tab or on another device (player tab), copy/paste or type in the URL that is shown on screen in the previous tab to join a room
4. repeat step 3 until you have reached the desired number of players for a quiz
5. back in your host tab, select a quiz to use from the dropdown menu
6. in the host tab, press **Start Quiz** once you have selected your quiz
7. in each player tab you used to **join the room**, answer the question that appears on your screen (you only have 30 seconds to answer)
8. once the game is over you may click the "Back to Home" button you see on screen

**Note:** the quiz will continue even if the tab that you used to create the room has been closed.
