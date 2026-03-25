# Pathfinder AI 🚀

A modern full-stack career guidance platform built with React, Vite, Node.js, Express, and MongoDB. Navigate your career path with AI-powered insights, real-time tech news, and personalized recommendations powered by Google Gemini AI.

## 🌟 Features

### 🎯 **Career Guidance Module**
- **AI-Powered Career Analysis**: Intelligent system that analyzes your skills, interests, and education using Google Gemini 1.5 Flash
- **Personalized Recommendations**: Get customized career path suggestions with confidence scoring
- **Skill Assessment**: Add and manage your professional skills
- **Real-time Typing Animation**: Dynamic display of career suggestions
- **User Authentication**: Secure JWT-based authentication system
- **Career History**: Save and track your career analysis results
- **Dark/Light Mode**: Toggle between themes with persistent storage

### 📊 **Career Dashboard**
- **High-Fidelity UI**: Career DNA dashboard with career progression tracking
- **Visual Analytics**: Beautiful charts and metrics
- **Career Pathways**: Explore different career options
- **Progress Tracking**: Monitor your career development

### 🌌 **Galaxy-Themed Landing Page**
- **Cosmic Design**: Stunning space-themed aesthetics with animated backgrounds
- **Multiple Sections**:
  - Loading Screen with animated rings
  - Hero Section with neon text effects
  - Features Section highlighting AI capabilities
  - Tech News integration with Google News RSS
  - CTA Section with pricing plans
  - Footer with links
- **Framer Motion Animations**: Smooth, performant animations throughout

### 📰 **Live Tech News**
- **Google News RSS Integration**: Real-time technology news feed
- **Backend Processing**: Server-side RSS parsing and caching
- **Automatic Updates**: Refreshes every 5 minutes
- **Responsive Display**: News card integrated into Features section

### 📖 **Academic Roadmap**
- **Multi-Stage Guidance**: Tailored paths for Class 10, 12, Undergraduate, and Postgraduate students
- **Plan A & Plan B Options**: Primary career paths + contingency alternatives for competitive fields
- **Actionable Milestones**: Immediate next steps for each educational stage
- **Career Path Exploration**: 3-4 trending options per stage with descriptions
- **Alternative Routes**: "What if?" toggle showing backup career paths with reasoning tooltips
- **Skill Development**: Specific skills to focus on at each milestone
- **Interactive Tabs**: Smooth transitions between different academic stages
- **Visual Differentiation**: Cyan borders for Plan B mode vs Purple/Pink for Plan A
- **Galaxy Theme Integration**: Glassmorphism cards with neon borders and animations

### 🔐 **Authentication System**
- **JWT Authentication**: Secure token-based authentication
- **Password Hashing**: bcryptjs for secure password storage
- **Protected Routes**: API endpoints secured with middleware
- **User Management**: Registration and login functionality
- **Session Management**: Persistent user sessions with token refresh

### 🎨 **Unified Navigation System**
- **Smart Navbar**: Context-aware navigation across all pages
- **Active Page Highlighting**: Visual indicator of current page
- **Mobile Responsive**: Hamburger menu for smaller screens
- **Theme Toggle**: Global dark/light mode switch
- **Smooth Transitions**: Motion animations for all interactions
- **Active Page Highlighting**: Visual indicator of current page
- **Mobile Responsive**: Hamburger menu for smaller screens
- **Theme Toggle**: Global dark/light mode switch
- **Smooth Transitions**: Motion animations for all interactions

## 🛠️ **Tech Stack**

### **Frontend**
| Technology | Purpose |
|-----------|---------|
| **React 18.2.0** | UI framework |
| **Vite 5.4.21** | Build tool & dev server |
| **Tailwind CSS 3.4.1** | Utility-first styling |
| **Framer Motion 10.16.0** | Animation library |
| **Lucide React** | Icon library |
| **Axios 1.5.2** | HTTP client for API calls |

### **Backend**
| Technology | Purpose |
|-----------|---------|
| **Node.js 18+** | Runtime environment |
| **Express 4.18.2** | Web server framework |
| **MongoDB** | NoSQL database |
| **Mongoose 7.4.1** | MongoDB object modeling |
| **JWT 9.0.1** | Authentication tokens |
| **bcryptjs 2.4.3** | Password hashing |
| **Google Gemini 1.5 Flash** | AI career analysis |
| **rss-parser 3.12.0** | News feed parsing |

### **Security & Middleware**
| Technology | Purpose |
|-----------|---------|
| **Helmet 7.0.0** | Security headers |
| **CORS** | Cross-origin resource sharing |
| **express-rate-limit 7.0.0** | Rate limiting |
| **express-validator 7.0.1** | Input validation |

### **Development Tools**
| Technology | Purpose |
|-----------|---------|
| **PostCSS** | CSS processing |
| **ESLint** | Code linting |
| **Nodemon 3.1.14** | Development auto-restart |
| **dotenv 16.3.1** | Environment variables |

## 📁 **Project Structure**

```
d:\rit2/
├── backend/
│   ├── controllers/
│   │   ├── authController.js      # Authentication logic
│   │   ├── careerController.js    # Career analysis endpoints
│   │   └── newsController.js      # News feed management
│   ├── middleware/
│   │   ├── authMiddleware.js      # JWT authentication middleware
│   │   └── errorHandler.js        # Global error handling
│   ├── models/
│   │   ├── User.js                # User schema
│   │   └── CareerResult.js        # Career analysis storage
│   ├── routes/
│   │   ├── authRoutes.js          # Authentication routes
│   │   ├── careerRoutes.js        # Career analysis routes
│   │   └── newsRoutes.js          # News routes
│   ├── services/
│   │   ├── authService.js         # Authentication business logic
│   │   ├── careerService.js       # Career analysis orchestration
│   │   ├── geminiService.js       # Google Gemini AI integration
│   │   └── newsService.js         # RSS news processing
│   ├── .env                       # Environment variables
│   ├── .env.example               # Environment template
│   ├── package.json               # Backend dependencies
│   ├── package-lock.json          # Dependency lock file
│   └── server.js                  # Express server entry point
├── src/
│   ├── components/
│   │   ├── dashboard/
│   │   │   ├── PathfinderDashboard.jsx
│   │   │   ├── ProgressBar.jsx
│   │   │   ├── CareerCard.jsx
│   │   │   └── SkillGapChart.jsx
│   │   ├── landing/
│   │   │   ├── LoadingScreen.jsx
│   │   │   ├── HeroSection.jsx
│   │   │   ├── FeaturesSection.jsx
│   │   │   ├── AcademicGuide.jsx
│   │   │   ├── CTASection.jsx
│   │   │   ├── Footer.jsx
│   │   │   ├── GalaxyBg.jsx
│   │   │   └── TechNews.jsx
│   │   ├── CareerGuidance.jsx
│   │   └── Navbar.jsx
│   ├── pages/
│   │   ├── Landing.jsx
│   │   └── CareerGuidance.jsx
│   ├── data/
│   │   └── mockData.js
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── vite.config.js
├── tailwind.config.js
├── postcss.config.js
├── package.json
└── README.md
```

## 🚀 **Getting Started**

### Prerequisites
- **Node.js**: v18.0.0 or higher
- **npm**: v9.0.0 or higher
- **MongoDB**: Local installation or MongoDB Atlas account

### Installation

1. **Clone or navigate to project directory**
```bash
cd d:\rit2
```

2. **Set up environment variables**

**Frontend (.env in root directory):**
```bash
VITE_API_BASE_URL=http://localhost:5000/api
```

**Backend (.env in backend directory):**
```bash
JWT_SECRET=your_super_secure_jwt_secret_key_here
MONGODB_URI=mongodb://localhost:27017/pathfinder-ai
GEMINI_API_KEY=your_google_gemini_api_key_here
PORT=5000
```

Get your Gemini API key from: https://makersuite.google.com/app/apikey

3. **Install frontend dependencies**
```bash
npm install
```

4. **Install backend dependencies**
```bash
cd backend
npm install
cd ..
```

5. **Start MongoDB** (if running locally)
```bash
# Windows PowerShell
mongod --dbpath "C:\data\db"
```

6. **Start the backend server**
```bash
cd backend
npm run dev
```
Backend will be available at `http://localhost:5000`

7. **Start the frontend development server** (in a new terminal)
```bash
npm run dev
```
Frontend will be available at `http://localhost:5173`

### Build for Production

**Frontend:**
```bash
npm run build
```

**Backend:**
```bash
cd backend
npm run start
```

### API Endpoints

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/api/auth/register` | User registration | No |
| POST | `/api/auth/login` | User login | No |
| POST | `/api/career/analyze` | Career analysis | Yes |
| GET | `/api/news` | Get tech news | No |

## 📖 **Architecture Overview**

### **Backend Architecture**
- **server.js**: Express server with middleware stack (CORS, Helmet, Rate Limiting)
- **MongoDB Connection**: Automatic retry logic with 5-second intervals
- **JWT Authentication**: Bearer token validation middleware
- **Error Handling**: Global error handler with structured JSON responses
- **Input Validation**: express-validator for all API endpoints

### **Frontend Architecture**
- **App.jsx**: Main application shell with routing and theme management
- **API Integration**: Axios client for backend communication
- **State Management**: React hooks with localStorage persistence
- **Theme System**: Global dark/light mode with localStorage

### **CareerGuidance.jsx** - AI Career Advisor
- Form validation with real-time error feedback
- Skill management with add/remove functionality
- **Backend API integration** for AI-powered career analysis
- Typing animation for results display
- User authentication integration
- Career history tracking
- Intelligent fallback system if API is unavailable

### **Landing Page Components**
- **LoadingScreen.jsx**: Animated intro with spinning rings
- **HeroSection.jsx**: Main hero with gradient text and CTA buttons
- **FeaturesSection.jsx**: Feature grid with AI capability highlights
- **TechNews.jsx**: Live tech news from backend API
- **CTASection.jsx**: Pricing plans and conversion section
- **GalaxyBg.jsx**: Reusable cosmic background with 6 animation layers
- **Footer.jsx**: Links and contact information

### **PathfinderDashboard.jsx** - Career Dashboard
- Career progression visualization
- Metrics and analytics display
- Career pathway recommendations
- Beautiful card-based layout

## 🤖 **Backend Services Architecture**

### **geminiService.js** - AI Analysis Engine
The backend service handles all AI-powered career recommendations:

```
Frontend Request → careerController.js
  ↓
Authentication Check (authMiddleware.js)
  ↓
Input Validation (express-validator)
  ↓
careerService.js Orchestration
  ↓
geminiService.js API Call
  ↓
Google Gemini 1.5 Flash API
  ↓
JSON Response Processing
  ↓
Database Storage (CareerResult model)
  ↓
Structured Response to Frontend
```

**Key Functions**:
- `getCareerAnalysis()`: Main entry point for career analysis
- `callGeminiAPI()`: Secure API call with error handling
- `parseGeminiResponse()`: Safely extracts JSON from API response
- `saveCareerResult()`: Stores analysis in MongoDB
- `getFallbackSuggestions()`: Intelligent fallback when API unavailable

**Features**:
- Server-side API key protection
- Error handling with graceful degradation
- Smart fallback based on keywords if API fails
- Confidence scoring for each suggestion
- Education-level aware recommendations
- Career history persistence

### **authService.js** - Authentication Service
```
User Registration/Login → authController.js
  ↓
Input Validation
  ↓
Password Hashing (bcryptjs)
  ↓
JWT Token Generation
  ↓
Database Storage (User model)
  ↓
Token Response
```

### **newsService.js** - News Aggregation Service
```
GET /api/news → newsController.js
  ↓
RSS Feed Fetching
  ↓
XML Parsing (rss-parser)
  ↓
Article Filtering & Formatting
  ↓
JSON Response
```

## 🎯 **Features In Detail**

### Career Guidance Analysis
The AI analyzes user input using **Google Gemini 1.5 Flash API** to generate intelligent, personalized career suggestions based on:
- **User Skills**: High-weight matching (direct relevance)
- **Career Interests**: Medium-weight matching (contextual alignment)
- **Education Level**: Low-weight matching (program prerequisites)

The system generates 3 contextually relevant career suggestions with:
- Career title and trajectory overview
- Personalized reasoning based on user input
- Recommended next skills to develop
- Confidence score (percentage match)
- **Persistent storage** in MongoDB for user history

**Smart Fallback**: If the Gemini API is unavailable, the system falls back to an intelligent keyword-based recommendation engine to ensure continuous service.

### Authentication System
- **JWT-based authentication** with secure token storage
- **Password hashing** using bcryptjs (12 salt rounds)
- **Protected API routes** with middleware validation
- **User registration and login** with input validation
- **Token expiration** (7 days) with refresh capability
- **Secure password requirements** (minimum 6 characters)

### Database Integration
- **MongoDB** with Mongoose ODM
- **User model**: Email, hashed password, timestamps
- **CareerResult model**: User reference, analysis data, timestamps
- **Connection retry logic** for reliability
- **Data validation** at schema level

### Gemini API Integration
- **Backend Service**: `backend/services/geminiService.js`
- **API Model**: Google Gemini 1.5 Flash (fast, cost-efficient)
- **Security**: Server-side API key protection
- **Processing**: Structured JSON responses with error handling
- **Fallback System**: Intelligent keyword-based suggestions when API fails

### Tech News Integration
- Fetches from: `https://news.google.com/rss/search?q=technology`
- **Backend Processing**: Server-side RSS parsing with rss-parser
- Updates automatically every 5 minutes
- Displays up to 6 latest articles with publication dates
- **Public API endpoint**: No authentication required

### Rate Limiting & Security
- **15 requests per 15 minutes** per IP address
- **Helmet.js** security headers
- **CORS** configuration for cross-origin requests
- **Input validation** on all API endpoints
- **Error sanitization** to prevent information leakage

## 🎨 **Design System**

### Color Palette
- **Primary**: Purple (#8b5cf6), Pink (#ec4899)
- **Secondary**: Cyan (#06b6d4)
- **Dark Mode**: Slate-900, Slate-800, Slate-700
- **Light Mode**: Gray-50, White

### Typography
- **Font Family**: Poppins, System fonts
- **Headings**: Bold, large sizes (3xl-5xl)
- **Body**: Regular weight, readable sizes

### Spacing
- **Consistent**: 4px base unit (Tailwind default)
- **Padding**: 4px, 8px, 16px, 24px increments
- **Gaps**: 8px-32px for component spacing

## 🔧 **Configuration Files**

### **Frontend Configuration**

**vite.config.js**
- React fast refresh plugin
- Development server configuration
- Port fallback handling

**tailwind.config.js**
- Extended color definitions
- Custom animations (galaxy effects)
- Typography scales

### **Backend Configuration**

**server.js**
- Express server setup with middleware stack
- MongoDB connection with retry logic
- Route mounting and error handling

**package.json**
- ES modules support (`"type": "module"`)
- Development script with nodemon
- Production dependencies for security and performance

### **Environment Variables**

**.env (Frontend)**
```
VITE_API_BASE_URL=http://localhost:5000/api
```

**.env (Backend)**
```
JWT_SECRET=your_super_secure_jwt_secret_key_here
MONGODB_URI=mongodb://localhost:27017/pathfinder-ai
GEMINI_API_KEY=your_google_gemini_api_key_here
PORT=5000
```

- Never commit `.env` files to version control
- Use `.env.example` as templates
- Get Gemini API key from: https://makersuite.google.com/app/apikey
- Custom animations (galaxy effects)
- Typography scales

### **tailwind.css**
- Custom CSS variables
- Global animations
- Reusable utility classes

## 📊 **Performance Optimizations**

- **Code Splitting**: Component-based lazy loading
- **Memoization**: React.memo for expensive components
- **Lazy Effects**: useEffect cleanup for interval management
- **CSS Optimization**: Tailwind JIT compilation
- **Build Optimization**: Vite minification and chunking

## 🌐 **Browser Support**

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 **Usage Examples**

### **Access Landing Page**
```
http://localhost:5173
```
- Scroll through sections
- Click "Career Guidance" to navigate

### **User Registration**
```bash
POST /api/auth/register
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "securepassword123"
}
```

### **User Login**
```bash
POST /api/auth/login
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "securepassword123"
}

// Response includes JWT token
{
  "token": "eyJhbGciOiJIUzI1NiIs...",
  "user": { "id": "...", "email": "user@example.com" }
}
```

### **Use Career Guidance Tool**
1. Register/Login to get authentication token
2. Navigate to Career Guidance page
3. Fill in your details:
   - Full Name
   - Education Level
   - Career Interests (describe what interests you)
   - Skills (add multiple skills with "+" button)
4. Click "Get Career Advice"
5. Wait for AI analysis (2-second animation)
6. View your personalized career recommendation
7. **Results are automatically saved** to your account history

### **Get Tech News**
```bash
GET /api/news
Authorization: Bearer your_jwt_token

// Returns latest technology news articles
[
  {
    "title": "Latest Tech News",
    "link": "https://...",
    "pubDate": "2024-01-15T10:30:00Z"
  }
]
```

### **Switch Themes**
- Click the Sun/Moon icon in navbar
- Theme persists across sessions

### **Access Dashboard**
- Click "Dashboard" in navbar
- View career progression metrics

## 🐛 **Troubleshooting**

### Port Already in Use
```bash
# Frontend: Vite automatically tries next available port
# Check console output for correct port (usually 5174, 5175, 5176...)

# Backend: Kill process using port 5000
netstat -ano | findstr :5000
taskkill /pid <PID> /f
```

### MongoDB Connection Issues
- Ensure MongoDB is running locally or check your MongoDB Atlas connection string
- Verify `MONGODB_URI` in backend `.env` file
- Check MongoDB logs for connection errors

### Authentication Errors
- Verify JWT_SECRET is set in backend `.env`
- Check token expiration (7 days default)
- Ensure Authorization header format: `Bearer <token>`

### Gemini API Issues
- Verify `GEMINI_API_KEY` is set in backend `.env`
- Check API key validity at https://makersuite.google.com/app/apikey
- Monitor API quota and rate limits

### Theme Not Persisting
- Clear browser localStorage: `localStorage.clear()`
- Check if "theme" key exists in DevTools

### Tech News Not Loading
- Verify internet connection
- Check backend server is running
- Try refreshing the page or wait 5 minutes for auto-update

### Forms Not Saving
- Ensure user is authenticated
- Check backend server logs for validation errors
- Verify MongoDB connection for data persistence

### CORS Errors
- Ensure backend CORS configuration allows frontend origin
- Check VITE_API_BASE_URL in frontend `.env`

### Rate Limiting
- Wait 15 minutes after hitting the limit (15 requests per 15 minutes)
- Check response headers for rate limit information

## 📚 **Key Libraries Documentation**

- **React**: https://react.dev
- **Vite**: https://vitejs.dev
- **Tailwind CSS**: https://tailwindcss.com
- **Framer Motion**: https://www.framer.com/motion/
- **Lucide React**: https://lucide.dev

## 🤝 **Contributing**

To add new features:
1. Create components in appropriate directory
2. Follow existing naming conventions
3. Use Tailwind CSS for styling
4. Implement dark mode support
5. Add error handling and loading states
6. Test responsiveness

## 📄 **File Size**

- Production Build: ~150-200KB (gzipped)
- Node Modules: ~500MB
- Source Code: ~50KB

## 🔐 **Security Considerations**

- Form data stored locally only
- No sensitive data sent to external APIs (RSS proxy is read-only)
- XSS protection via React's built-in escaping
- CORS handled via trusted proxy service

## 📞 **Support**

For issues or questions:
- Check the [Troubleshooting](#-troubleshooting) section
- Review component documentation in code comments
- Check browser console for error messages

## 📅 **Version History**

- **v2.0.0** (March 25, 2026)
  - Full-stack architecture with Node.js/Express backend
  - MongoDB integration with Mongoose ODM
  - JWT authentication system
  - Google Gemini AI integration moved to backend
  - Career analysis persistence and user history
  - RSS news processing on backend
  - Security middleware (Helmet, CORS, Rate Limiting)
  - Input validation and error handling
  - Production-ready backend with clean architecture

- **v1.0.0** (March 24, 2026)
  - Initial release
  - Career Guidance module
  - Galaxy-themed landing page
  - Live tech news integration
  - Dark/Light theme support
  - Unified navigation system

## 📜 **License**

This project is built as a demonstration of modern full-stack development practices with React, Node.js, and MongoDB.

---

**Built with ❤️ using React, Vite, Node.js, Express, and MongoDB**

**Last Updated**: March 25, 2026
