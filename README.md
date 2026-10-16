# Hackathon Runners website

This is a static website. Keep `index.html`, `style.css`, and `script.js` at the repository root; no package installation or build command is required.

## Deploy on Vercel

1. Push the repository to GitHub.
2. In Vercel, choose **Add New Project** and import the repository.
3. Use the **Other** framework preset and leave the build command empty.
4. Deploy. Vercel serves `index.html` and its relative CSS/JavaScript assets from the project root.

## Admin prototype limitation

Admin credentials and content are stored in the current browser's local storage. First-time setup suggests the username `onkar`; passwords must be at least 8 characters and include uppercase, lowercase, and numeric characters. The credential hash is salted, but the sign-in check and all admin code are delivered to visitors in JavaScript. This is not secure authentication, does not synchronize between visitors, and must not be used to protect private content. Secure shared admin access requires server-side authentication and persistent storage.
