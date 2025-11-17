# Learning Plus — Static Website

A small static website for Learning Plus — a simple educational site with registration and account pages. This repository contains the HTML and CSS files used to build the site and is suitable for learning, prototyping, or small static hosting.

**Status:** Ready for local preview and minor improvements.

**Quick Links:**
- `learnigplus.html` — Main landing / registration page
- `acount.html` — Create new account page
- `learnigplus.css` — Styles used by the main page
- `acount.css` — Styles used by the account page

**Preview:** Open the HTML files directly in your browser or serve the folder with a simple static server (instructions below).

---

**Project Layout**

- `learnigplus.html` — Main website with signup, feedback, and links to the account page.
- `acount.html` — Standalone form for creating a new account (uses `student.css` reference in the file; stylesheet file for account is `acount.css` in the repo).
- `learnigplus.css` — CSS for the main page layout and components.
- `acount.css` — CSS for the account form and responsive form styles.
- `README.md` — This file.

---

**How to Preview Locally**

Method 1 — Open file directly

1. In File Explorer, double-click `learnigplus.html` or `acount.html` to open them in your default browser.

Method 2 — Use a simple HTTP server (recommended for testing relative links)

Open PowerShell in the project folder and run:

```powershell
python -m http.server 8000
# then open http://localhost:8000/learnigplus.html in your browser
```

Or using PowerShell's built-in `Start-Process` to open the file directly:

```powershell
Start-Process .\learnigplus.html
```

---

**Notes & Suggestions**

- The account page (`acount.html`) links to `student.css` in its `<head>` but the repository includes `acount.css`. You may want to update the `<link>` in `acount.html` to reference `acount.css` for consistent styling.
- Image assets are referenced via external URLs. For offline use, download images into an `assets/` folder and update the `<img>` `src` attributes.
- Consider renaming files to correct typos (`acount.html` → `account.html`, `learnigplus.css` → `learningplus.css`) if you want cleaner names — note this will require updating links in HTML files.

---

**Contributing**

Feel free to open issues or submit pull requests for enhancements such as:

- Fixing typos in filenames and HTML (`acount` → `account`, `learnigplus` → `learningplus`).
- Improving responsive layout and accessibility (labels, aria attributes, form validations).
- Adding a small build/preview dev script (npm or Makefile) if you intend to expand the project.

---

**License**

This project contains simple example files; add a license file if you intend to publish or share the project under specific terms.

---

**Contact / Author**

Created as a small static site prototype. For questions or collaboration, update the repo or send a message to the project maintainer.
