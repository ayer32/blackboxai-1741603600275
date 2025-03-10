# Modern Portfolio Website

A modern, responsive portfolio website built with HTML, Tailwind CSS, and JavaScript.

## Features
- Modern UI/UX design with animations and glassmorphism effects
- Responsive layout for all devices
- Profile picture upload with validation
- Interactive project cards and skill indicators
- Contact form with validation
- Dark/Light mode support
- Smooth scrolling and transitions

## Running Locally

1. Clone the repository:
```bash
git clone <your-repo-url>
cd portfolio-website
```

2. Option 1: Using Python's built-in server
```bash
# If you have Python 3 installed
python3 -m http.server 8000

# If you have Python 2 installed
python -m SimpleHTTPServer 8000
```
Then open http://localhost:8000 in your browser.

3. Option 2: Using Node.js's http-server
```bash
# Install http-server globally
npm install -g http-server

# Run the server
http-server -p 8000
```
Then open http://localhost:8000 in your browser.

4. Option 3: Using VS Code's Live Server extension
- Install the "Live Server" extension in VS Code
- Right-click on index.html and select "Open with Live Server"

## Deployment Options

1. GitHub Pages
```bash
# Create a new repository on GitHub
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-github-repo-url>
git push -u origin main

# Enable GitHub Pages in your repository settings
# Select the main branch as source
```
Your site will be available at: https://<your-username>.github.io/<repo-name>

2. Netlify
- Sign up for a free account at netlify.com
- Connect your GitHub repository
- Select the repository and branch to deploy
- Your site will be deployed automatically

3. Vercel
```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel
```

4. Firebase Hosting
```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login to Firebase
firebase login

# Initialize Firebase project
firebase init hosting

# Deploy
firebase deploy
```

## Customization

1. Update personal information in index.html:
- Name and title
- About section
- Skills and expertise
- Project details
- Contact information

2. Replace profile picture:
- Upload your profile picture
- Update the src attribute in the img tag

3. Update CV:
- Replace the CV file in the assets folder
- Update the download link href

4. Customize colors:
- Update the Tailwind configuration in the style section
- Modify color variables for primary and secondary colors

5. Add/Remove sections:
- Each section is clearly marked with comments
- Copy existing section structure for new sections
- Remove unwanted sections

## Production Build

For production deployment:

1. Optimize images:
```bash
# Using npm package imagemin-cli
npm install -g imagemin-cli
imagemin images/* --out-dir=dist/images
```

2. Minify CSS:
- Replace the Tailwind CDN with a production build
- Follow Tailwind's [installation guide](https://tailwindcss.com/docs/installation)
- Run `npx tailwindcss -o dist/style.css --minify`

3. Minify JavaScript:
```bash
# Using terser
npm install -g terser
terser script.js -o dist/script.min.js
```

4. Update asset references to use minified versions

## Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## Contributing
Feel free to fork this repository and submit pull requests for improvements.

## License
MIT License - feel free to use this template for your own portfolio.
