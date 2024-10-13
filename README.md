# 🌐 URL Shortener

Welcome to the **URL Shortener** application! This tool allows users to shorten long URLs into more manageable links. You can access the live application at [ktzr.lol](https://ktzr.lol).

## 🛠️ Setup Instructions

### Prerequisites

- Ensure that [Node.js](https://nodejs.org/) and [MongoDB](https://www.mongodb.com/) are installed on your system.

### 1. Clone the Repository

```bash
git clone https://github.com/Omria09/url-shortener-fullstack.git
cd url-shortener-fullstack
git submodule init
git submodule update
```

### 2. Backend Setup

1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Install the required dependencies:
   ```bash
   npm install
   ```
3. Add a `.env` file in the `backend` directory with the following content:
   ```
   MONGO_URI=mongodb+srv://<username>:<password>@/<clutter>.mongodb.net/<dbname>?retryWrites=true&w=majority&appName=url-shortener-db
   ```
4. Start MongoDB:
   ```bash
   mongod
   ```
5. Run the backend server:
   ```bash
   node server.js
   ```

### 3. Frontend Setup

1. Navigate to the `frontend` directory:
   ```bash
   cd ../frontend
   ```
2. Install the frontend dependencies:
   ```bash
   npm install
   ```
3. Add a `.env.local` file in the `frontend` directory with the following content:
   ```
   REACT_APP_API_BASE_URL=http://localhost:5000/api/
   ```
4. Start the frontend development server:
   ```bash
   npm start
   ```

## 🚀 Running the Application

1. Ensure the backend (`mongod` and `node server.js`) is running.
2. Ensure the frontend (`npm start`) is running.
3. Open your web browser and navigate to:
   - **Local Development**: [http://localhost:3000](http://localhost:3000)
   - **Live Version**: [ktzr.lol](https://ktzr.lol)

## 🧪 Testing the Application

To run tests for this application:

Fronted:

1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Launch the test runner:
   ```bash
   npm test
   ```
   This will run all tests in `App.test.js`.

Backend:

1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Launch the test runner:
   ```bash
   npm test
   ```
   This will run all tests in `url.test.js`.

## 📜 Available Scripts

Inside the `frontend` and `backend` directories, the following scripts are available:

- **`npm start`**: Runs the app in development mode.
- **`npm test`**: Runs the test suite in watch mode.
- **`npm run build`**: Builds the app for production in the `build` folder.
- **`npm run eject`**: Ejects the app, allowing for full configuration control.

Feel free to reach out for contributions or issues!
