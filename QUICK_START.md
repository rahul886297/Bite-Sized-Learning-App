# Quick Start Guide

## 1. Install Dependencies

### Backend
```bash
cd backend
npm install
```

### Frontend
```bash
cd frontend
npm install
```

## 2. Setup Environment

### Backend
Create `backend/.env`:
```
PORT=5000
JWT_SECRET=your_super_secret_key_change_in_production
NODE_ENV=development
DATABASE_PATH=../database/app.db
```

## 3. Database Setup

Seed with sample data:
```bash
cd backend
npm run seed
```

## 4. Start Development Servers

### Terminal 1 - Backend
```bash
cd backend
npm start
# or with auto-reload
npm run dev
```

Backend runs on: http://localhost:5000

### Terminal 2 - Frontend
```bash
cd frontend
npm start
```

Frontend runs on: http://localhost:3000

## 5. Login with Demo Account

- **Email**: john@example.com
- **Password**: creator123
- **Role**: Creator (can upload videos)

## 6. Test Features

### As a Creator:
1. Log in with demo account
2. Go to "Upload" page
3. Upload a test video
4. Create a course and add videos
5. View analytics in Progress page

### As a Student:
1. Register new account with role "student"
2. Browse video feed
3. Generate AI summaries and quizzes
4. Create playlists
5. Track progress

## Available Scripts

### Backend
- `npm start` - Start server
- `npm run dev` - Start with nodemon
- `npm run seed` - Seed database

### Frontend
- `npm start` - Start development server
- `npm run build` - Build for production
- `npm test` - Run tests

## Troubleshooting

### Port Already in Use
- Backend (5000): `lsof -i :5000` and kill the process
- Frontend (3000): `lsof -i :3000` and kill the process

### Database Issues
- Delete `database/app.db` and run `npm run seed` again

### CORS Errors
- Ensure backend is running on http://localhost:5000
- Check frontend is on http://localhost:3000

### Can't Login
- Run seed script again: `npm run seed`
- Try demo credentials: john@example.com / creator123

## Next Steps

1. **Explore the code** - Check out the architecture in README.md
2. **Read the pitch deck** - See vision in docs/PITCH_DECK.md
3. **Test the API** - Use Postman/Insomnia with Bearer token auth
4. **Customize** - Modify colors, add features, improve UI

Happy learning! 🚀
