
# 🏒 NHL Player Analysis Tool 📊

This is a web application for tracking, analyzing, and comparing NHL hockey players and teams, built with React frontend and Flask backend. The application was designed to be used by my team and I to assist in making data-driven decisions regarding player and team evaluation.


## Table of Contents

- [Quickstart and Installation](#quickstart-and-installation)
- [Features](#features)
- [How to Use](#how-to-use)
- [Project Structure](#project-structure)
- [FAQ](#faq)
## Quickstart and Installation

### Prerequisites
- Node.js (v16 or higher)
- Python 3.7 or higher
- pip (Python package manager)

### 1. Install Dependencies

```bash
# Install all dependencies (both frontend and backend)
npm install

# Or install separately:
npm run install-backend    # Python dependencies
npm run install-frontend   # React dependencies
```

### 2. Initialize Database

```bash
# Create database with sample players
npm run init-db
```

### 3. Start the Application

```bash
# Start both frontend and backend simultaneously
npm run dev

# Or start separately:
npm run start-backend    # Flask API (port 5000)
npm run start-frontend   # React app (port 3000)
```

### 4. Open Your Browser

- Frontend: http://localhost:3000
- Backend API: http://localhost:5001
## Features

- **View All Players** - use card-based layout to view players and teams at a glance
- **In-Depth View** - select a player or team to view more advanced stats
- **Compare** - Compare player and team statistics one on one to determine superior performance
- **Add New Players** - As new players enter the league, you can update your data sets with name, team, position, and stats
- **Real-time Updates** - when adding new players or updating stats
## Usage Examples

### Launch App
![Launch App](https://github.com/wooly11/TC497-README-Assignment/blob/main/run_app.gif)

### Add a Player
![Add a Player](https://github.com/wooly11/TC497-README-Assignment/blob/main/add_player.gif)
## Project Structure

### Tech Stack
- **Frontend**: React 19, CSS3
- **Backend**: Flask (Python)
- **Database**: SQLite
- **Styling**: Custom CSS with modern design

### Architecture Diagram
![Architecture Diagram](https://github.com/wooly11/TC497-README-Assignment/blob/main/Architecture%20Diagram.png)

### File Descriptions
```
hockey-analysis/
├── app.py                # Flask backend server
├── init_db.py            # Database initialization script
├── requirements.txt      # Python dependencies
├── package.json          # Node.js dependencies and scripts
├── players.db            # SQLite database (created after init)
└── hockey-frontend/      # React frontend application
    ├── src/
    │   ├── App.js        # Main React component
    │   └── App.css       # Styling
    └── package.json      # Frontend dependencies
```
## FAQ

#### What are my API endpoints?
- `GET /health` - Health check endpoint
- `GET /players` - Get all players
- `POST /players` - Add a new player

#### How do I reset the database if I am having issues?
```bash
# Remove existing database and recreate with sample data
npm run init-db
```

#### Why am I getting errors with my ports?
Make sure ports 3000 and 5000 are available and not already in use. Switch to available port if necessary.

#### Why am I getting CORS errors?
The backend is configured to allow requests from localhost:3000

