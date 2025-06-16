# 📊 Math-A-Day Quiz

A modern, interactive web application that presents users with a fresh high-school level math problem every day. Problems are dynamically generated using Google's Gemini AI and cached locally for optimal performance.

## ✨ Features

### 🎯 Core Functionality
- **Daily Problem Generation**: Automatically generates a unique math problem each day using Gemini 2.0 Flash API
- **Smart Caching**: Problems are stored in localStorage to avoid regenerating on the same day
- **Multiple Input Types**: Supports both multiple choice questions and free-form text input
- **Intelligent Answer Checking**: Handles numerical answers with floating-point tolerance and string normalization

### 🎨 User Interface
- **Responsive Design**: Fully responsive layout that works on desktop, tablet, and mobile devices
- **Modern Styling**: Clean, contemporary design using Tailwind CSS with smooth animations
- **Mathematical Notation**: Integrated MathJax for proper rendering of mathematical expressions
- **Visual Feedback**: Color-coded responses, loading states, and progress indicators

### 🧮 Problem Types
- **Algebra**: Linear equations, quadratics, polynomials
- **Geometry**: Area, perimeter, angles, coordinate geometry
- **Trigonometry**: Basic trig functions, identities, applications
- **Statistics & Probability**: Basic statistical concepts and probability problems

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/math-a-day-quiz.git
   cd math-a-day-quiz
   ```

2. **Get a Gemini API Key**
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Generate a new API key for Gemini 2.0 Flash

3. **Configure the API Key**
   - Open `index.html` in a text editor
   - Find line 87: `this.apiKey = "";`
   - Replace with your API key: `this.apiKey = "your-api-key-here";`

4. **Launch the Application**
   - Open `index.html` in your web browser
   - Or serve it using a local server:
     ```bash
     python -m http.server 8000
     # Navigate to http://localhost:8000
     ```

## 🛠️ Technical Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Tailwind CSS (CDN)
- **Math Rendering**: MathJax
- **AI Integration**: Google Gemini 2.0 Flash API
- **Storage**: Browser localStorage
- **Architecture**: Single-page application (SPA)

## 📱 Browser Compatibility

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

## 🔧 How It Works

1. **Daily Check**: On page load, the app checks if a problem exists for the current date
2. **Problem Generation**: If no problem exists, it calls the Gemini API with a structured prompt
3. **Response Processing**: The API returns a JSON object with question, answer, explanation, and options
4. **Local Storage**: The problem is cached locally with the current date
5. **User Interaction**: Users can answer via multiple choice or text input
6. **Feedback & Learning**: Immediate feedback is provided with detailed explanations

## 📊 API Schema

The application uses a structured JSON schema for consistent problem generation:

```json
{
  "id": "unique-problem-id",
  "question": "What is the value of x in 2x + 5 = 11?",
  "options": ["x = 2", "x = 3", "x = 4", "x = 5"],
  "answer": "x = 3",
  "explanation": "To solve 2x + 5 = 11, subtract 5 from both sides...",
  "topic": "Algebra",
  "difficulty": "Easy"
}
```

## 🎯 Key Features

### For Students
- **Daily Practice**: Consistent math practice with varied problems
- **Instant Feedback**: Know immediately if your answer is correct
- **Detailed Explanations**: Step-by-step solutions for learning
- **Mobile Friendly**: Practice anywhere, anytime

### For Educators
- **Curriculum Aligned**: High-school level problems across key topics
- **Self-Contained**: No backend required, easy to deploy
- **Customizable**: Easy to modify problem types and difficulty

### For Developers
- **Clean Architecture**: Well-structured, commented code
- **Modern JavaScript**: ES6+ features with async/await
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **API Integration**: Example of AI service integration

## 🔐 Privacy & Security

- **No Personal Data**: No user information is collected or stored
- **Local Storage Only**: All data stays in the user's browser
- **API Key Security**: Remember to keep your API key secure and consider server-side implementation for production

## 🚀 Deployment Options

### Static Hosting
- **GitHub Pages**: Perfect for personal projects
- **Netlify**: Easy deployment with form handling
- **Vercel**: Fast global CDN deployment

### Local Development
- **File Protocol**: Open directly in browser for testing
- **Local Server**: Use Python, Node.js, or any static server

## 🤝 Contributing

Contributions are welcome! Here are some ways to help:

1. **Bug Reports**: Found an issue? Please report it
2. **Feature Requests**: Have an idea? Let's discuss it
3. **Code Improvements**: Submit PRs for enhancements
4. **Documentation**: Help improve the docs

### Development Setup

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Submit a pull request with a clear description

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google Gemini AI** for providing the problem generation capabilities
- **MathJax** for beautiful mathematical notation rendering
- **Tailwind CSS** for the responsive design framework
- **The Math Education Community** for inspiration and feedback


Made with ❤️ for math enthusiasts everywhere. Happy problem solving! 🧮✨
