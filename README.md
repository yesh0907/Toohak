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
1. in a browswer tab, navigate to http://localhost:5173/ and create a room
2. in another browswer tab, copy and paste the url that is shown on screen in the previous tab to join a room
3. repeat step 3 until you have reached the desired number of players for a quiz
4. back in your first browswer tab, select a quiz you would like to use
5. press start quiz once you have selected your quiz
6. in each tab you used to **join the room**, answer the question that appears on your screen (you only have 30 seconds to answer)
7. once the game is over you may click the "Back to Home" button you see on screen


**Note:** the quiz will continue even if the tab that you used to create the room has been closed.