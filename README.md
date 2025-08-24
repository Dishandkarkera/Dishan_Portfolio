# Dishan_Portfolio — Local server instructions

Form submission on this portfolio uses FormSubmit (https://formsubmit.co). FormSubmit and many other features require the site to be served over HTTP or HTTPS and will not work when the HTML file is opened directly via the `file://` protocol in the browser.

To run the site locally and test the contact form, serve the project directory with a simple web server and open `http://localhost:8000` (or the port you choose).

Recommended quick options (PowerShell on Windows):

- Using Python (if Python is installed):

```powershell
# from the project root (where index.html lives)
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

- Using Node (npx serve):

```powershell
npx serve . -l 8000
# then open http://localhost:8000
```

Notes:
- If you still see the site opened with `file://`, the page will display a banner indicating FormSubmit won't work and the contact form submit button will be temporarily disabled. Use the mailto fallback shown in the contact info or start a local server and reload the page.
- For production, host the site on any static host (GitHub Pages, Netlify, Vercel, etc.) and FormSubmit will work normally.

If you'd like, I can also add a small PowerShell script to start a server or add a GitHub Pages configuration to publish the site automatically.
