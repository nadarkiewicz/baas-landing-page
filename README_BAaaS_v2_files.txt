BAaaS v2 site files

Copy these files into your Astro project root:

D:\Projects\BAaaS\landing-page\src\config\site.ts
D:\Projects\BAaaS\landing-page\src\layouts\Layout.astro
D:\Projects\BAaaS\landing-page\src\styles\global.css
D:\Projects\BAaaS\landing-page\src\pages\index.astro
D:\Projects\BAaaS\landing-page\src\pages\pl\index.astro

Then in VS Code:
1. Open folder: D:\Projects\BAaaS\landing-page
2. Open Terminal inside VS Code: Ctrl + `
3. Run:
   npm run build
4. If build succeeds, use VS Code Source Control to commit and sync, or run:
   git status
   git add .
   git commit -m "Update landing page to v2"
   git push

Analytics:
- GA is optional.
- Empty gaMeasurementId means no GA loads and the page still works.
- Put your GA ID in src/config/site.ts when ready:
  gaMeasurementId: "G-XXXXXXXXXX"

Lead magnet form:
- Current fallback opens an email draft.
- For real lead capture, paste a form endpoint into leadMagnetAction in src/config/site.ts.
