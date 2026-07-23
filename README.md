# Eric Zhao — Portfolio [Website](https://ericsjsu-datascience.github.io/portfolio/)

A clean, responsive, JSON-driven portfolio website built using **HTML**, **TailwindCSS**, and **JavaScript**.  
The site is deployed with **GitHub Pages** and designed to organize and present my projects, experience, skills, and education.

All content is modularized into `/data/*.json` files for easy maintenance—no need to edit HTML structure.



---

## 🚀 Features

### **Dynamic JSON-Driven Content**
All major sections fetch data dynamically:

- `projects.json`
- `experience.json`
- `education.json`
- `skills.json`
- `status_badge.json`

This separates content from UI, making updates simple and clean.

### **Responsive Interface**
- Built with TailwindCSS CDN  
- Supports mobile, tablet, laptop  
- Smooth dark/light theme toggle (saved in localStorage)

### **Rotating Profile Photos**
A timed crossfade animation cycles through multiple images using JavaScript.

### **Interactive Contact Section**
- “Email” button supports **click-to-copy**
- GitHub & LinkedIn links included



---

## 📁 Repository Structure

```
portfolio/
│
├── index.html # Main webpage (renders JSON data)
│
├── assets/
│ ├── img/ # Profile & other photos
│ └── Eric_Zhao_Resume.pdf
│
├── data/ # All editable content
│ ├── projects.json
│ ├── experience.json
│ ├── education.json
│ └── status_badge.json
│
└── README.md
```



---

## 🛠 Local Development

Because this site uses `fetch()` to load JSON,  
you **cannot** open `index.html` directly with `file:///`.

### **Option 1 — VS Code Live Server (recommended)**
1. Install **Live Server** extension  
2. Right-click `index.html` → **Open with Live Server**  
3. Visit `http://localhost:5500`

### **Option 2 — Python local server**

```python -m http.server 8000```

Then open:

```http://localhost:8000```



---

## 🌐 Deployment (GitHub Pages)

1. Go to **Settings → Pages**
2. Select:
   - Branch: `main`
   - Folder: `/root`
3. Save  
4. GitHub will automatically publish your site



---

## ✏️ How to Update Content

### **Update Projects**
Edit `/data/projects.json`:

```json
[
  {
    "title": "project name",
    "type": "Academic/Personal/something else",
    "desc": [
      "bulletpoint 1",
      "bulletpoint 2",
      "bulletpoint 3"
    ],
    "link": "https://github.com/example"
  }
]
```

### **Update Experience**

Modify `/data/experience.json`.

### **Update Education**

Modify `/data/education.json`.

### **Update Status Badges**

Modify `/data/status_badge.json`.

### **Update Skills**

Modify `/data/skills.json`.

Still need better way to represent skills.



---

## 📬 Contact

[Email](vet.ericzhao@gmail.com)

[GitHub](https://github.com/EricSJSU-DataScience)

[LinkedIn](https://www.linkedin.com/in/eric-zhao-data-scientist/)

---



## ✅ To-Do: 

- ~~re-orgnize project section and add to portfolio~~
- ~~add skill section~~
- ~~add project section (general info should enough for now)~~
- ~~move contents to `data` folder `.json` files, index.html script will fetch `.json`~~
- ~~complete readme.md~~
- ~~re-work for skill section~~
- find better way to present skill section