# Publish Retro Bowl Modded as a website

This is a static website. The game and mod menu are loaded from `index.html`, `html5game/RetroBowl.js`, and `mod-menu.js`. No database or backend server is required for the basic site.

## Test locally on Windows

1. Install Node.js LTS from https://nodejs.org/ if it is not installed.
2. Extract this ZIP. Open PowerShell in the `retro-bowl-modded-main` folder.
3. Run `npm install` once.
4. Run `npm start`.
5. Open the local URL printed in PowerShell (usually `http://localhost:3000`). Keep the terminal open while testing.

You can also use VS Code's Live Server extension, but serving the folder over HTTP is recommended over opening `index.html` directly.

## Publish it online with Netlify

1. Extract the ZIP on your computer.
2. Go to https://app.netlify.com/drop and sign in.
3. Drag the **`retro-bowl-modded-main` folder's contents** (the files inside it, including `index.html`, `html5game`, `img`, `saves`, and `mod-menu.js`) into the deploy area. If the page accepts only a ZIP, zip the folder contents first and upload that ZIP.
4. Wait for deployment, then open the generated `*.netlify.app` address.

## Publish with Vercel

1. Create a repository in GitHub and upload the contents of this folder.
2. Import that repository at https://vercel.com/new.
3. Choose no build command and set the output/public directory to `.` (the project root). Deploy.

## Important notes

- This package includes an unofficial fan-made game project and game assets. Only publish it if you have the rights/permission to distribute all included files and comply with the original game's terms. Hosting it publicly may create copyright or trademark issues; the project's existing disclaimer does not itself grant those rights.
- Save data is handled by the browser; it is not automatically shared between devices or browsers.
- Test the game, mod menu, save import/export, and starter-save prompt on the deployed URL.
