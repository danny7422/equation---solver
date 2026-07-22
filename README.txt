SIMULTANEOUS EQUATION SOLVER — APP PACKAGE
==========================================

WHAT'S IN THIS FOLDER
  index.html                the solver (also works standalone, offline, double-click to open)
  manifest.webmanifest      app identity: name, icon, colours
  sw.js                     service worker — makes the app work fully offline once installed
  icon-192.png              app icons
  icon-512.png
  icon-maskable-512.png
  README.txt                this file

You can use index.html on its own forever by just double-clicking it.
The steps below are only needed to INSTALL it as an app on your phone
and PC with its own icon.


STEP 1 — HOST IT (one time, free, ~10 minutes)
----------------------------------------------
Installable apps must be served over https, so the files need to live
on a web host. GitHub Pages is free and permanent.

  1. Go to github.com and sign in (create a free account if needed).
  2. Click the + (top right) -> "New repository".
     Name it e.g.  equation-solver   and set it to Public. Create.
  3. On the new repository page click "uploading an existing file".
  4. Drag ALL the files in this folder in (not the folder itself —
     the individual files, so index.html sits at the top level).
     Click "Commit changes".
  5. Go to Settings -> Pages (left sidebar).
     Under "Branch" choose  main  and  / (root),  then Save.
  6. Wait a minute, refresh, and GitHub shows your address:
         https://YOURNAME.github.io/equation-solver/
     That address is your app. It never expires and costs nothing.


STEP 2 — INSTALL ON YOUR ANDROID PHONE
--------------------------------------
  1. Open the address in Chrome.
  2. Either tap the "Install app" button that appears in the solver's
     button row, or Chrome menu (⋮) -> "Add to Home screen" -> Install.
  3. It appears on your home screen with the Σx icon, opens
     full-screen like any app, and works with no signal at all.

  iPhone: open in Safari -> Share -> "Add to Home Screen".


STEP 3 — INSTALL ON YOUR PC
---------------------------
  1. Open the address in Chrome or Edge.
  2. Click the install icon at the right end of the address bar
     (a monitor with a down-arrow), or menu -> "Install app".
  3. It gets its own window, taskbar icon, and Start-menu entry,
     and works offline.


UPDATING THE APP LATER
----------------------
  1. Edit index.html (or ask Claude for a new version).
  2. In sw.js change   solver-v1   to   solver-v2.
  3. Upload both files to the repository again (same drag-and-drop,
     "Commit changes"). Installed copies pick up the new version the
     next time they are opened twice.


NOTES
-----
- Everything runs on the device. No data is sent anywhere; there is
  no server-side code and no account.
- Print sheet -> "Save as PDF" gives a filed calculation record with
  the title block (project, ref, initials, date).
- Lines starting with # are comments — label your ΣFx / ΣFy / ΣM
  blocks directly in the input.
