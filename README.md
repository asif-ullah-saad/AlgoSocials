# EchoBreaker - Break Out of Your Social Media Echo Chamber

EchoBreaker is a modern web application that helps users break out of social media echo chambers by analyzing their information diet, visualizing it, and suggesting diverse perspectives.

## 🎯 Features

- **Information Diet Analysis**: Analyze your social media feed to understand your exposure to different viewpoints
- **Bubble Score**: Calculate a score (0-100) based on feed diversity to quantify echo chamber exposure
- **Interactive Visualizations**: Beautiful charts showing political leaning distribution and topic analysis
- **Challenge Mode**: Engage with opposing viewpoints through guided challenges and reflection exercises
- **Content Suggestions**: Get personalized recommendations for diverse, credible sources
- **AI-Powered Nudges**: Intelligent suggestions to fact-check claims and explore primary sources
- **User Dashboard**: Comprehensive overview of your information diet and progress
- **Social Media Integration**: Connect Twitter and Instagram accounts (mock integration for now)

## 🚀 Tech Stack

- **Framework**: Next.js 14 with TypeScript
- **Styling**: Tailwind CSS with custom design system
- **Authentication**: Clerk for secure user authentication
- **Charts**: Chart.js with react-chartjs-2 for data visualization
- **Icons**: Lucide React for modern icons
- **State Management**: React hooks and context
- **Deployment**: Vercel-ready

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd echobreaker
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env.local` file in the root directory:
   ```env
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🔧 Configuration

### Clerk Authentication Setup

1. Sign up for a free account at [clerk.com](https://clerk.com)
2. Create a new application
3. Copy your publishable key and secret key
4. Add them to your `.env.local` file

### Tailwind CSS

The project uses Tailwind CSS with a custom design system. The configuration is in `tailwind.config.js` and includes:

- Custom color palette (primary blues, secondary greens)
- Custom animations and transitions
- Responsive design utilities
- Custom component classes

## 📁 Project Structure

```
src/
├── app/                    # Next.js app directory
│   ├── api/               # API routes
│   ├── dashboard/         # Dashboard page
│   ├── challenges/        # Challenges page
│   ├── settings/          # Settings page
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   └── page.tsx           # Home page
├── components/            # React components
│   ├── charts/           # Chart components
│   ├── dashboard/        # Dashboard-specific components
│   ├── challenges/       # Challenge components
│   └── layout/           # Layout components
├── lib/                  # Utility functions
├── types/                # TypeScript type definitions
└── middleware.ts         # Clerk middleware
```

## 🎨 Design System

### Colors
- **Primary**: Blue gradient (#3B82F6 to #1E40AF)
- **Secondary**: Green gradient (#22C55E to #16A34A)
- **Neutral**: Gray scale for text and backgrounds

### Components
- **Cards**: Clean, rounded cards with subtle shadows
- **Buttons**: Primary and secondary button styles
- **Forms**: Consistent input styling with focus states
- **Charts**: Interactive charts with hover effects

## 🔍 Key Components

### BubbleScoreCard
Displays the user's bubble score with a circular progress indicator and suggestions for improvement.

### InformationDietChart
Interactive pie chart showing the distribution of political leanings in the user's feed.

### ChallengeCard
Allows users to complete challenges with reflection questions and stores responses locally.

### ContentSuggestions
Recommends diverse sources based on the user's information diet analysis.

## 🚀 Deployment

### Vercel Deployment

1. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Deploy to Vercel**
   - Connect your GitHub repository to Vercel
   - Add environment variables in Vercel dashboard
   - Deploy automatically on push

### Environment Variables for Production

Make sure to set these in your Vercel dashboard:
- `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`
- `CLERK_SECRET_KEY`

## 🧪 Testing

The application includes comprehensive error handling and loading states. To test:

1. **Authentication Flow**: Test sign-in/sign-out functionality
2. **Dashboard**: Verify data loading and chart rendering
3. **Challenges**: Complete challenges and check local storage
4. **Settings**: Test notification preferences and account management

## 🔒 Security

- **Authentication**: Secure user authentication with Clerk
- **Data Privacy**: User data is stored locally (localStorage) for challenges
- **API Protection**: All API routes are protected with authentication middleware
- **Environment Variables**: Sensitive keys are stored in environment variables

## 📊 Data Flow

1. **User Authentication**: Clerk handles user authentication
2. **Feed Analysis**: Mock data is generated for demonstration
3. **Bubble Score Calculation**: Algorithm calculates diversity score
4. **Content Suggestions**: Recommendations based on feed analysis
5. **Challenge Completion**: Stored locally for persistence

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Clerk](https://clerk.com) for authentication
- [Chart.js](https://chartjs.org) for data visualization
- [Tailwind CSS](https://tailwindcss.com) for styling
- [Lucide](https://lucide.dev) for icons

## 📞 Support

For support, email support@echobreaker.com or create an issue in the GitHub repository.

---

**EchoBreaker** - Breaking echo chambers, one perspective at a time. 🎯

