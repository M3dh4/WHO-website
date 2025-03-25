# World Health Organization Website

This guide provides simplified instructions for collaborating on the WHO Health Predictor mini project using a single main branch approach.

## Getting Started

### Prerequisites
- Install Node.js and npm from [nodejs.org](https://nodejs.org/)
- Install Git from [git-scm.com](https://git-scm.com/downloads)
- Create a GitHub account at [github.com](https://github.com/)

### Setting Up Git
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Accessing the Repository

1. **Clone the repository**:
   ```bash
   git clone https://github.com/YOUR-USERNAME/WHO-website.git
   cd WHO-website
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Run the application**:
   ```bash
   npm start
   ```

## Working on the Project

### Before Making Changes
Always pull the latest changes before starting work:
```bash
git pull origin main
```

### Making and Submitting Changes

1. **Make your changes** to your assigned page
2. **Test your changes** locally
3. **Commit your changes**:
   ```bash
   git add .
   git commit -m "Add description of your changes"
   ```
4. **Push to main**:
   ```bash
   git pull origin main  # Get any new changes first
   # Resolve any conflicts if they occur
   git push origin main
   ```

## Integration Guidelines

### Navigation Integration
The header navigation is already set up in the main App.js file. To integrate your page:

1. Create your page component in `src/components/pages/`
2. Import and add your component to App.js:

```jsx
// In App.js
import YourPage from './components/pages/YourPage';

// In the return statement, add a route for your page
// Look for the existing navigation items and follow the same pattern
```

### Styling Guidelines
- Use the existing color scheme (dark blue #003366 for headers)
- Maintain the black world map with red dots for the Health Predictor page
- Support both dark/light mode using the MODE toggle
- Support language switching with the EN dropdown

### Theme and Language Support
All pages should:
- Work with both dark and light modes
- Support language switching
- Use the shared header component


