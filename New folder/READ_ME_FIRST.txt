LAKHAN CONSTRUCTION — SITE REGISTER (installable app)
========================================================

WHAT'S IN THIS FOLDER
----------------------
index.html               The app itself
manifest.webmanifest      Tells the browser this is an installable app
sw.js                     Service worker — makes the app work offline
icon-192.png              App icon (home screen / taskbar)
icon-512.png              App icon (larger, app stores/splash screens)
icon-512-maskable.png     App icon (Android adaptive icon shape)
apple-touch-icon.png      App icon for iPhone/iPad

IMPORTANT — KEEP ALL FILES TOGETHER
-------------------------------------
These files must stay in the SAME folder for the app to install and
work offline. If you only keep index.html by itself, the app will
still run completely normally — it just won't offer "Install" or
work without internet.

HOW TO MAKE IT INSTALLABLE (pick one, both are free)
-------------------------------------------------------

OPTION A — Netlify Drop (easiest, 2 minutes, no account needed)
  1. Go to https://app.netlify.com/drop in your browser
  2. Drag this whole folder onto the page
  3. You'll get a live https:// web address instantly
  4. Open that address on your phone or PC —
     you'll now see an "Install" option (Chrome/Edge/Android)
     or you can "Add to Home Screen" (iPhone: Share button → Add to Home Screen)

OPTION B — GitHub Pages (if you already use GitHub)
  1. Create a new repository and upload all the files in this folder
  2. Go to Settings → Pages → set source to the main branch
  3. GitHub gives you a live https:// address — open it and install as above

WHY HOSTING IS NEEDED
------------------------
Browsers only allow "Install app" and offline mode on pages loaded
over https:// (or from a proper local server) — not on a file you've
just downloaded and double-click to open. This is a browser security
rule, the same for every website, not something specific to this app.

If you'd rather NOT host it online, you can still just open index.html
directly like before — all your worker/attendance/advance data will
keep saving normally either way. You just won't get the app icon or
offline support without hosting it.

YOUR DATA
-----------
Your data is saved on whichever device/browser you use the app from.
It is not affected by any of the above — hosting the files online does
not upload your worker data anywhere; it only makes the app itself
installable. Keep downloading the Excel backup from the Export tab
regularly either way.
