# Rural Learning Quest 🎓

An interactive educational platform for rural students with gamified learning experience.

## Features ✨

- 🎮 Interactive Quizzes across multiple subjects
- 🏆 Leaderboard system with real-time rankings
- 📝 Personal note-taking system
- ✅ To-do list for task management
- 🎯 Achievement badges
- ⏱️ Study time tracker
- 🌙 Dark mode support
- 📱 Fully responsive design

## Tech Stack 🛠️

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Backend**: Node.js, Express.js
- **Database**: SQLite3
- **Authentication**: JWT, bcrypt

## Quick Start 🚀

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/rural-learning-quest.git
cd rural-learning-quest
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory:
```env
PORT=5000
JWT_SECRET=your-super-secret-key-change-this
NODE_ENV=development
```

4. Start the server:
```bash
npm start
```

5. Open your browser and visit:
```
http://localhost:5000
```

## Deployment 🌐

### Deploy to Render.com (Recommended)

1. Push your code to GitHub

2. Create a new Web Service on Render.com

3. Connect your GitHub repository

4. Configure the service:
   - **Build Command**: `npm install`
   - **Start Command**: `npm start`
   - **Environment Variables**:
     - `JWT_SECRET`: Generate a secure random string
     - `NODE_ENV`: `production`

5. Click "Create Web Service"

Your app will be live at: `https://your-app-name.onrender.com`

### Deploy to Heroku

```bash
# Install Heroku CLI
# Login to Heroku
heroku login

# Create new app
heroku create your-app-name

# Set environment variables
heroku config:set JWT_SECRET=your-secret-key
heroku config:set NODE_ENV=production

# Deploy
git push heroku main
```

## Project Structure 📁

```
rural-learning-quest/
├── server-sqlite.js          # Main backend server
├── api-integration.js        # Frontend API connector
├── package.json              # Dependencies
├── .env                      # Environment variables (not in git)
├── .gitignore               # Git ignore rules
├── render.yaml              # Render deployment config
├── public/                  # Frontend files
│   └── index.html          # Main HTML file
└── README.md               # This file
```

## API Endpoints 📡

### Authentication
- `POST /api/register` - Register new user
- `POST /api/login` - Login user

### User
- `GET /api/profile` - Get user profile (auth required)
- `PUT /api/gamestate` - Update game progress (auth required)
- `GET /api/stats` - Get user statistics (auth required)
- `DELETE /api/account` - Delete account (auth required)

### Public
- `GET /api/leaderboard` - Get leaderboard
- `GET /api/health` - Health check

## Environment Variables 🔐

| Variable | Description | Required |
|----------|-------------|----------|
| PORT | Server port (default: 5000) | No |
| JWT_SECRET | Secret key for JWT tokens | Yes |
| NODE_ENV | Environment (development/production) | Yes |

## Development 💻

### Run in development mode:
```bash
npm run dev
```

### Database
SQLite database file (`rural-learning-quest.db`) is created automatically on first run.

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request.

## License 📄

This project is licensed under the MIT License.

## Support 📧

If you encounter any issues, please open an issue on GitHub.

## Acknowledgments 🙏

- Built for rural education initiatives
- Designed to work in low-bandwidth environments
- Focused on accessibility and ease of use

---

Made with ❤️ for rural students
