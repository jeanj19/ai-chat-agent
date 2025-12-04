# AI Agent Chat - Frontend

Next.js frontend for the AI Agent Chat Application. This is the user interface that connects to the FastAPI backend to provide an interactive chat experience with OpenAI GPT-4.

## Features

- **Modern Chat Interface**: Clean, responsive design with Material-UI
- **Conversation Management**: Create, switch between multiple conversations
- **Real-time Messaging**: Interactive chat with AI agent
- **Mobile Responsive**: Works seamlessly on desktop and mobile
- **Custom Theming**: Dark gradient theme with consistent styling
- **TypeScript**: Full type safety throughout the application

## Tech Stack

- **Next.js 16**: React framework
- **React 19**: UI library
- **TypeScript**: Type safety
- **Material-UI**: Component library
- **Lucide React**: Icons
- **React Markdown**: Markdown rendering

## Getting Started

1. **Install dependencies:**
```bash
npm install
```

2. **Run development server:**
```bash
npm run dev
```

3. **Open browser:**
Navigate to [http://localhost:3000](http://localhost:3000)

## Project Structure

```
agent-ui/
├── components/          # React components
│   ├── ChatArea.tsx    # Main chat interface
│   ├── ChatMessage.tsx # Individual message display
│   ├── Sidebar.tsx     # Conversation navigation
│   └── WelcomeScreen.tsx # Initial screen
├── pages/              # Next.js pages
│   ├── index.tsx       # Main dashboard
│   └── _app.tsx        # App configuration
├── styles/             # CSS modules and themes
│   ├── theme/          # Custom theme system
│   └── *.module.css    # Component styles
└── public/             # Static assets
```

## Key Components

- **Dashboard**: Main layout with sidebar and chat area
- **ChatArea**: Handles message sending and display
- **Sidebar**: Conversation list and navigation
- **ChatMessage**: Individual message rendering with markdown support
- **WelcomeScreen**: Initial user interface

## API Integration

The frontend communicates with the FastAPI backend running on `http://localhost:8001`:

- `POST /agent` - Send messages to AI
- `GET /conversations` - Fetch conversation list
- `POST /conversations` - Create new conversation
- `GET /conversations/{id}/messages` - Get conversation history

## Styling

Uses a custom theme system with:
- CSS custom properties for consistent theming
- Material-UI integration
- Responsive design patterns
- Dark gradient backgrounds

## Development

- **Hot Reload**: Automatic page updates during development
- **TypeScript**: Full type checking and IntelliSense
- **ESLint**: Code quality and consistency
- **CSS Modules**: Scoped styling

**Note**: Make sure the FastAPI backend is running on port 8001 for full functionality.
