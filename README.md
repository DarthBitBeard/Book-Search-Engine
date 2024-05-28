# Book Search Engine

This is a full-stack application that allows users to search for books using the Google Books API and save their favorite books. It includes user authentication, allowing users to sign up, log in, save books, and view their saved books.

## Technologies Used

- Node.js
- Express
- MongoDB
- Mongoose
- React
- Bootstrap
- Heroku (for deployment)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/google-books-search-app.git
   cd google-books-search-app
   ```

2. Install server dependencies:
   ```sh
   cd server
   npm install
   ```

3. Install client dependencies:
   ```sh
   cd ../client
   npm install
   ```

4. Create a `.env` file in the root of the `server` directory and add your MongoDB URI:
   ```
   MONGODB_URI=your-mongodb-uri
   ```

## Running the Application Locally

1. Start the MongoDB server:
   ```sh
   mongod
   ```

2. Start the server:
   ```sh
   cd server
   npm start
   ```

3. In a new terminal, start the client:
   ```sh
   cd client
   npm start
   ```

4. Open your browser and go to `http://localhost:3001` to view the application.

## Deploying to Heroku

1. Log in to Heroku:
   ```sh
   heroku login
   ```

2. Create a new Heroku application:
   ```sh
   heroku create your-app-name
   ```

3. Set up environment variables on Heroku:
   ```sh
   heroku config:set MONGODB_URI=your-mongodb-uri
   ```

4. Add, commit, and push your code to Heroku:
   ```sh
   git add .
   git commit -m "Initial commit"
   git push heroku main
   ```

5. Open your application in a web browser:
   ```sh
   heroku open
   ```

## Directory Structure

```
client/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── utils/
│   ├── App.css
│   ├── App.jsx
│   ├── index.js
│   └── ... (other React files)
server/
├── config/
├── controllers/
├── models/
├── routes/
├── utils/
├── server.js
└── ... (other server files)
```

## License

This project is licensed under the MIT License.
