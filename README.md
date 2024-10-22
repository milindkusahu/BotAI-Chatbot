# BotAI Chatbot

A modern, interactive chatbot application built with ReactJS that enables users to have conversations with an AI model and provide multi-dimensional feedback. The application features a clean, intuitive interface with comprehensive feedback mechanisms and conversation management.

![Chat Interface](public/screenshots/chat-interface.png)

## Features

### Core Functionality

- Interactive chat interface with AI responses (using mock data)
- Real-time conversation feedback system
  - Thumbs up/down reactions for individual responses
  - 5-star rating system for overall conversation quality
  - Subjective feedback collection at conversation end
- Conversation history management
- Feedback analytics dashboard with filtering capabilities

![Feedback Dashboard](public/screenshots/feedback-dashboard.png)

### Additional Features

- Light/Dark mode toggle
- Responsive design for all screen sizes
- Clean and intuitive user interface
- Conversation persistence and retrieval
- Advanced feedback filtering and sorting

## Demo

![Dark Mode](public/screenshots/dark-mode.png)
*Dark Mode View with Chat History*

## Tech Stack

- **Frontend Framework:** React.js
- **UI Components:** Material-UI
- **State Management:** React Context API
- **Styling:** Tailwind CSS
- **Icons:** Material Icons
- **Data Storage:** Local Storage
- **Deployment:** Vercel

## Data Implementation

This application uses a mock data approach instead of real API integration:

- Responses are stored in a JSON file
- No API key or external service required
- Predictable responses for testing and demonstration
- Easy to modify or extend the response dataset

```javascript
// Sample response data structure
{
  "responses": [
    {
      "question": "Hello",
      "answer": "Hi! How can I help you today?"
    },
    {
      "question": "How are you?",
      "answer": "I'm functioning well, thank you! How can I assist you?"
    }
    // ... more response pairs
  ]
}
```

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager

### Installation

1. Clone the repository

```bash
git clone https://github.com/milindkusahu/BotAI-Chatbot.git
```

2. Navigate to the project directory

```bash
cd BotAI-Chatbot
```

3. Install dependencies

```bash
npm install
# or
yarn install
```

4. Start the development server

```bash
npm run dev
# or
yarn dev
```

5. Open your browser and visit `http://localhost:3000`

## Technical Decisions

### Why React?

- Component reusability
- Virtual DOM for efficient rendering
- Rich ecosystem of libraries
- Strong community support
- Easy state management with Context API

### Why Material-UI?

- Comprehensive component library
- Consistent design language
- Built-in responsiveness
- Easy theme customization
- Accessibility support out of the box

### Why Local Storage?

- Simplified data persistence
- No backend required
- Quick setup for prototype
- Instant data access
- Offline capability

### Why Mock Data?

- No dependency on external APIs
- Consistent behavior for testing
- Quick development and prototyping
- No API key management required
- Easy to modify responses

## Design Decisions

### User Interface

- Clean and minimalist design for better focus on conversations
- Floating feedback buttons to reduce visual clutter
- Sidebar for easy access to conversation history
- Intuitive navigation between different views
- Clear visual hierarchy in feedback dashboard

![Mobile View](public/screenshots/mobile-view.png)
*Responsive Mobile View*

### User Experience

- Progressive feedback collection to avoid overwhelming users
- Immediate response to user interactions
- Smooth transitions between different states
- Consistent theme across all components
- Clear visual indicators for interactive elements

## Trade-offs and Future Improvements

### Current Trade-offs

1. Using local storage instead of a backend database

   - Pro: Simplified deployment and setup
   - Con: Limited storage capacity and data persistence
2. Mocked AI responses

   - Pro: Predictable behavior for testing
   - Con: Limited interaction possibilities
3. Client-side filtering

   - Pro: Quick response time
   - Con: May not scale well with large datasets

### Future Improvements

1. Backend Integration

   - Implement proper database storage
   - Add user authentication
   - Real AI model integration
2. Enhanced Features

   - Export feedback data
   - Advanced analytics dashboard
   - Conversation search functionality
   - Tags for conversation categorization
3. Performance Optimizations

   - Implement pagination for large datasets
   - Add lazy loading for conversation history
   - Optimize component rendering

## Deployment

The application is deployed on Vercel and can be accessed at: [BotAI Chatbot](https://bot-ai-chatbot.vercel.app/)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
