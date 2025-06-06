

````markdown
# Korean Auto Imports Website

A responsive, single-page marketing site for **Korean Auto Imports**, featuring sections like Home, About, Products, and Contact. Built using HTML, Tailwind CSS, and JavaScript, with extended functionality to parse and convert `.xlsx` files into CSV format.

---

## 🚀 Features

- **Responsive Design** using Tailwind CSS
- **Smooth Scrolling** for anchor navigation
- **Mobile Navigation Toggle**
- **Hero Section** with Parallax Background
- **Product Cards** showcasing automotive parts
- **Contact Section** with Email CTA
- **Dynamic `.xlsx` Parsing** with fallback for plain CSV
- **Cross-browser compatible**

---

## 📁 Project Structure

```plaintext
index.html       # Main HTML file with all content and embedded JavaScript
````

---

## 📦 Dependencies

* **Tailwind CSS CDN** – for utility-first responsive design
* **[SheetJS (XLSX.js)](https://cdn.sheetjs.com/)** – expected to be used but not included (you'll need to add the library if using `.xlsx` functionality)

**Note:** For the `loadFileData(filename)` function to work with `.xlsx` files, ensure you load `XLSX.js` in the `<head>`:

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
```

---

## 🧠 How It Works

### 1. Navigation & Layout

* Uses Tailwind CSS utility classes for layout and styling.
* Fixed navigation header with toggleable mobile menu.
* Smooth scrolling between sections using anchor tags and JavaScript.

### 2. XLSX File Parser

The JavaScript function `loadFileData(filename)` handles `.xlsx` files by:

* Reading the base64-encoded file
* Parsing the first sheet using SheetJS
* Automatically detecting and filtering out empty rows
* Extracting a heuristic-based header row
* Converting to CSV for display or processing

### 3. Interactivity

* Menu toggle for mobile
* Scroll animation for anchor links
* Mobile menu hides after selection

---
## Autor
--Ahmed Khaled
## 🛠️ Usage

1. Clone or download this repository.
2. Add it to your preferred web server or open `index.html` directly in the browser.
3. (Optional) Add XLSX.js library if `.xlsx` processing is needed.

---


