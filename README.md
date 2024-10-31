# 3D Portfolio Project for Architecture Client
Made By **Jamie Geddes**

This project is a 3D portfolio website created for an architecture client, showcasing projects, designs, and visual content in an engaging, interactive format.

## Project Overview

This portfolio site serves as a showcase for an architectural client, leveraging 3D models and interactive components to enhance the user experience. It is built with [Three.js, React, Tailwind, Vite, Blender, Github/Git Deployment.] and designed to be visually engaging and informative.

## Features

- **Interactive 3D Models**: Integrated 3D elements into the design.
- **Responsive Design**: Adapts to various screen sizes for mobile, tablet, and desktop.
- **Special Features**: Can zoom in on images in the modal for high quality viewing of architecture plans
- **Modern UI/UX**: Clean, minimalistic design aligned with contemporary architectural aesthetics.
- **GitHub Pages Deployment**: Easily deploy updates to GitHub Pages using `npm run deploy`.

## List of Packages
- @emailjs/browser@4.3.3
- @react-three/drei@9.108.3
- @react-three/fiber@8.16.8
- @splinetool/react-spline@4.0.0
- @types/react-dom@18.3.0
- @types/react@18.3.3
- @vitejs/plugin-react@4.3.1
- autoprefixer@10.4.19
- eslint-plugin-react-hooks@4.6.2
- eslint-plugin-react-refresh@0.4.8
- eslint-plugin-react@7.34.3
- eslint@8.57.0
- framer-motion@11.3.1
- gh-pages@6.1.1
- maath@0.10.8
- postcss@8.4.39
- react-dom@18.3.1
- react-image-zoom@1.3.1
- react-inner-image-zoom@3.0.2
- react-modal@3.16.1
- react-router-dom@6.24.1
- react-simple-maps@3.0.0
- react-tilt@1.0.2
- react-vertical-timeline-component@3.6.0
- react@18.3.1
- tailwindcss@3.4.4
- three@0.166.1
- vite@5.3.3



## How to Deploy For Future Guide

1. **Update credential manager if switching to this github account or use git config in bash**:
   
   This allows me to push to github deployment with right user account. If have multiple on PC can be wrong one logged in. 
   ```bash
   - git config user.email [ email ]
   - git config user.name [name]
   ```
     Also, confirm that the remote repository URL is correct by running:
     ```bash
     git remote -v
     ```
     Make sure you are in the correct branch for deployment.
2. **run npm run deploy in the terminal in the directory**:
   ```terminal
   - npm run deploy
   
** Note that you must be in the deployment branch for this to work

** You can also just run `npm run build` to build the project and test for errors before deploy

## How to Run Dev Server For Future Guide
1. **Run in visual studio code the following code to deploy**:
   ```bash
   - npm run dev

## Common Issues & Troubleshooting
**1. `npm run deploy` Errors**  
   - **Cause**: Node modules or GitHub Pages cache may be causing conflicts.
   - **Solution**: Clear the GitHub Pages cache:
     ```bash
     rm -rf node_modules/.cache/gh-pages
     ```
     Then try redeploying with `npm run deploy`.

**2. Development Server Not Starting**  
   - **Cause**: Dependencies are missing or incorrect Node version.
   - **Solution**: Ensure you have the correct Node version and all dependencies installed:
     ```bash
     node -v  # Verify Node version
     npm install  # Reinstall dependencies
     npm run dev  # Start the development server

**3. Incorrect `homepage` URL in `package.json`**  
   - **Cause**: The `homepage` field in `package.json` is set to the wrong URL, which can cause deployment issues.
   - **Solution**: Open `package.json` and check that the `homepage` field matches your GitHub Pages URL, like this:
     ```json
     "homepage": "https://elliottyoung1.github.io/Portfolio-Website/"
