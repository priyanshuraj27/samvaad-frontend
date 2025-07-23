# Samvaad - Frontend

A React-based debate platform built with Vite and Tailwind CSS.

## Features

- Debate screens for different formats (AP, BP, WS, One-on-One)
- User authentication and profiles
- Browse motions and debate topics
- Rebuttal trainer
- Custom adjudicator tools

## Tech Stack

- **React 19** - Frontend framework
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling framework
- **React Router DOM** - Client-side routing
- **Axios** - HTTP client
- **Lucide React** - Icons

## Local Development

1. Clone the repository
```bash
git clone https://github.com/priyanshuraj27/samvaad-frontend.git
cd samvaad-frontend
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
```bash
cp .env.example .env
```
Edit the `.env` file and set your API base URL:
```
VITE_API_BASE_URL=http://localhost:3000
```

4. Start the development server
```bash
npm run dev
```

The app will be available at `http://localhost:3000`

## Build

To build the application for production:

```bash
npm run build
```

The built files will be in the `dist` directory.

## Deployment to Vercel

This project is configured for deployment on Vercel:

1. **Deploy via Vercel CLI:**
```bash
npm install -g vercel
vercel
```

2. **Deploy via GitHub:**
   - Connect your GitHub repository to Vercel
   - Set the environment variable `VITE_API_BASE_URL` in your Vercel project settings
   - Vercel will automatically deploy on every push to main branch

3. **Environment Variables:**
   Make sure to set the following environment variable in your Vercel project:
   - `VITE_API_BASE_URL`: Your backend API URL

## Project Structure

```
src/
├── screen/           # All screen components
│   ├── login.jsx
│   ├── signup.jsx
│   ├── dashboard.jsx
│   ├── profile.jsx
│   ├── debate_screen.jsx
│   ├── APDebateScreen.jsx
│   ├── BPDebateScreen.jsx
│   ├── WSDebateScreen.jsx
│   ├── onevonedebate.jsx
│   ├── browsemotions.jsx
│   ├── rebuttaltrainer.jsx
│   ├── adjudicator.jsx
│   └── customadjudicator.jsx
├── utils/
│   └── axiosInstance.js  # Axios configuration
├── assets/           # Static assets
├── App.jsx          # Main app component
└── main.jsx         # App entry point
```

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally
- `npm run lint` - Run ESLint

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request
