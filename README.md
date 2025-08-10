# Reverend Insanity (Arabic) Web Scraper

This project is a Python-based web scraper designed to download and save chapters of the Arabic translation of the novel **Reverend Insanity**.
It uses **Selenium** to collect all chapter links from the source website, and **BeautifulSoup** to extract and format the chapter content into neatly styled HTML files.

> **⚠ Disclaimer:**
> This project was created for educational purposes only. Please support the translators and original authors by visiting and reading from the official source.
> All scraped content comes from **[ar-no.com](https://ar-no.com/)** — full credit goes to them for their translation and hosting of the Arabic version of Reverend Insanity.

---

## 📜 Features

* **Automated Link Extraction**: Uses Selenium to navigate the site and fetch chapter links for all six arcs.
* **BeautifulSoup Parsing**: Downloads and formats chapters into HTML with right-to-left Arabic styling.
* **Batch Download**: Option to download a single chapter, a whole arc, or all chapters.
* **Clean Styling**: Dark theme with Arabic-friendly fonts and text alignment.

---

## 🛠 Requirements

Make sure you have the following installed:

* Python 3.8+
* Google Chrome
* ChromeDriver (matching your Chrome version)
* Required Python packages:

```bash
pip install selenium beautifulsoup4 requests
```

---

## 📂 Project Structure

```
Reverend-Insanity-Arabic-Scraper/
│
├── ScrapRI.py        # Selenium scraper to get all chapter links
├── RI_main.py        # BeautifulSoup parser & HTML generator
├── Links/            # Saved chapter links for each arc
└── Reverend Insanity/
    ├── [Arc Folders] # HTML files of downloaded chapters
    └── description.txt
```

---

## 🚀 Usage

### 1️⃣ Extract Links from the Website

Run the **ScrapRI.py** script to collect all chapter links:

```bash
python ScrapRI.py
```

This will save `.txt` files in the `Links/` folder for each arc.

### 2️⃣ Download Chapters

Run **RI\_main.py** and choose from the available options:

```bash
python RI_main.py
```

You can:

* Download a single chapter (`getChapter()`)
* Download all chapters from a specific arc (`getFolderXChapters()`)
* Download the entire novel (`getAllChapters()`)

---

## 🎨 Output Example

The chapters are saved in HTML format with:

* **Right-to-left** text alignment
* **Readable Arabic font**
* **Dark mode** background

---

## 🙏 Credits

All novel content and translations are from **[ar-no.com](https://ar-no.com/)**.
This scraper is not affiliated with the site or its translators — please support them by visiting their platform.

---

Would you like me to also include a **Usage GIF** in this README that visually shows the scraper running? It would make the repo look more engaging.
