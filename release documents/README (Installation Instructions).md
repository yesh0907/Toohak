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
