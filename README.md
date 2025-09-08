# Dead Or Alive?

Real-time sleep tracker. Know who's awake before you knock. Firebase + vanilla JS.

## Features

- **Real-time sync** - Status updates appear instantly across all devices
- **User accounts** - Secure login system with password protection
- **Live dashboard** - See everyone's current sleep/wake status
- **Responsive design** - Works on desktop, tablet, and mobile
- **Cloud storage** - Data synced via Firebase Realtime Database

## Tech Stack

- Frontend: HTML5, CSS3, Vanilla JavaScript
- Backend: Firebase Realtime Database
- Hosting: Netlify
- Real-time: Firebase WebSocket connections

## Setup

1. Clone the repository
```bash
git clone https://github.com/yourusername/dead-or-alive.git
cd dead-or-alive
```

2. Create a Firebase project at [console.firebase.google.com](https://console.firebase.google.com)

3. Enable Realtime Database in test mode

4. Get your Firebase config and replace the config object in `index.html`:
```javascript
const firebaseConfig = {
    apiKey: "your-api-key",
    authDomain: "your-project.firebaseapp.com",
    databaseURL: "https://your-project-rtdb.firebaseio.com",
    projectId: "your-project-id",
    // ... other config
};
```

5. Deploy to any static hosting service (Netlify, Vercel, GitHub Pages)

## Usage

1. Visit the deployed app
2. Create an account by selecting your name and setting a password
3. Login to access the dashboard
4. Toggle your sleep status - others will see updates immediately
5. Check who's available before messaging or calling

## Architecture

- **Frontend**: Single-page application with vanilla JavaScript modules
- **Database**: Firebase Realtime Database with WebSocket connections
- **Authentication**: Simple password-based system (stored in Firebase)
- **State Management**: Real-time listeners update UI automatically

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test with your own Firebase project
5. Submit a pull request

## License

MIT License - see LICENSE file for details

## Demo

[Live Demo](https://dedoralive.netlify.app/)

---

Built for friend groups who want to respect each other's sleep schedules.
