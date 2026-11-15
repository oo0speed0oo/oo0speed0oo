# Hi, I'm Michael 👋

📍 **Saitama, Japan** | 🛠️ **Python & iOS developer** | 🎓 **B.A. Computer Science** | 🟢 **Open to work**

I'm a CS graduate and English teacher who has lived in Japan for 15 years. I build tools that solve my own problems, then share them. Lately that means **private, local-first tools**: they run on my own Linux box, use a local AI model through Ollama, and send nothing to the cloud.

**Residence status:** Spouse of a Permanent Resident (永住者の配偶者等). No work restrictions and no visa sponsorship needed.

> 🇯🇵 **日本語での自己紹介**
> はじめまして、マイケルです。埼玉県在住で、日本に住んで15年になります。コンピューターサイエンスの学位を持つ英語講師で、自分の困りごとを解決するためのツールを作っています。最近は、Ollama（ローカルAI）を使って、データを外部に送らず自分のパソコンだけで動くツールを作っています。現在、日本でバックエンド、ツール開発、iOS開発の仕事を探しています。在留資格は「永住者の配偶者等」で、就労制限はありません。日本語はJLPT N4レベルで、N3を目指して勉強中です。

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Swift](https://img.shields.io/badge/-Swift-FA7343?style=flat-square&logo=swift&logoColor=white) ![SwiftUI](https://img.shields.io/badge/-SwiftUI-006ED3?style=flat-square&logo=swift&logoColor=white) ![Flask](https://img.shields.io/badge/-Flask-000000?style=flat-square&logo=flask&logoColor=white) ![Ollama](https://img.shields.io/badge/-Ollama-000000?style=flat-square) ![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white) ![Xcode](https://img.shields.io/badge/-Xcode-147EFB?style=flat-square&logo=xcode&logoColor=white)

## 🧰 Tools I Built and Use

These are the projects I use myself. They run on my own machine and use a local AI model.

### 🎬 [reel2txt](https://github.com/oo0speed0oo/reel2txt)
Paste a video, post, web page, PDF or Reddit link. My Linux box downloads it, transcribes the speech (English and Japanese), reads on-screen text with OCR, summarizes it and files it into my projects. Private, runs over Tailscale.
*Python · yt-dlp · faster-whisper · ffmpeg · Playwright · Ollama · systemd*
**What it shows:** a multi-stage processing pipeline (download, transcribe, OCR, summarize, file) built from several tools, packaged with install and update scripts and run as a systemd service. It has a free-disk-space guard, an optional password, and is reachable only over Tailscale.

### 🎯 [job-scout](https://github.com/oo0speed0oo/job-scout)
A job-search dashboard that runs on my own machine. It searches with SearXNG, reads each page with a local Ollama model, and sorts jobs into Yes, Maybe and No. It has profiles, rules for remote work, days off and hours, a live log and a standalone HTML export. It never applies or logs in for me.
*Python (standard library only) · SearXNG · Ollama · single-file HTML interface*
**What it shows:** a full tool with a backend server, a JSON API and a browser interface, using no third-party dependencies. It is built carefully around security: localhost-only by default, write requests need a custom header, and cross-origin requests are rejected. It is honest about its limits, since pages that block scripts are skipped and reported, not bypassed.

### 🔎 [search-helper](https://github.com/oo0speed0oo/search-helper)
A local AI research helper. I type what I want to find out, review the generated search queries, and it searches, reads pages, rates each one, and writes an action plan with sources. It saves HTML, CSV and plain-text reports.
*Python (standard library only) · Ollama · SearXNG · systemd*
**What it shows:** a clean split into separate modules (server, search-and-judge runner, query writer), offline tests that use a fake AI and fake search so they run anywhere, and defense against prompt injection: page text is treated as data, and pages that try to instruct the AI are flagged. A person approves the queries before anything runs.

### 🗂️ [web-archive-tools](https://github.com/oo0speed0oo/web-archive-tools)
A web scraper and OCR toolkit for archiving articles and extracting text from images and PDFs, with Japanese and English OCR.
*Python · Tesseract*
**What it shows:** practical scripting for batch jobs: it resumes where it stopped, logs progress, and waits politely between requests.

## 📱 iOS Apps

- 📚 [**JLPTPrep**](https://github.com/oo0speed0oo/JLPTPrep) - Native iOS study app for JLPT N5 and N4: vocabulary, kanji and grammar quizzes with score tracking. I use it on my iPhone every day. *(Swift, SwiftUI)*
- 🌸 [**Hanako**](https://github.com/oo0speed0oo/Hanako) - A personal friendship assistant: stay present in the lives of the people who matter most. *(Swift, SwiftUI)*
- 🏘️ [**NeighborhoodSkout**](https://github.com/oo0speed0oo/NeighborhoodSkout) - Map your block and remember your neighbors: houses, residents, roles, birthdays. *(Swift, SwiftUI)*

## 🍎 Classroom Projects

I teach English at 212 English, and I build tools for my own students.

- 🎯 [**Bingo-Game**](https://github.com/oo0speed0oo/Bingo-Game) - Classroom bingo with picture cards and a text-to-speech caller, used in real English classes in Japan. *(Python, Kivy)*
- 👻 [**Doodle Alive**](https://github.com/oo0speed0oo/doodle-alive) - A Halloween web app: draw a monster on a worksheet, snap a photo, and watch it come alive in an animated scene. Runs fully in the browser, and photos never leave the device. *(HTML, JavaScript)*
- 🎒 [**ELSC Game**](https://github.com/oo0speed0oo/elsc-game) - "Beat the noise, pass the test." A top-down, Zelda-style game with online high scores. [**▶ Play in your browser**](https://oo0speed0oo.github.io/elsc-game/) *(Python, pygame)*
- 🤼 [**Home Wide Wrestling**](https://github.com/oo0speed0oo/home-wide-wrestling) - A NES-style wrestling game with four wrestlers, a full move set, three arenas and chiptune music. [**▶ Play in your browser**](https://oo0speed0oo.github.io/home-wide-wrestling/) *(Python, pygame)*

## 🈶 JLPTPrep Across Platforms

The same JLPT study app, rebuilt on three platforms:

- 🌐 [**JLPTPrep-Web**](https://github.com/oo0speed0oo/JLPTPrep-Web) - Browser version with unit filters and wrong-answer logging *(Flask)*
- 🖥️ [**JLPTPrep-Desktop**](https://github.com/oo0speed0oo/JLPTPrep-Desktop) - The original desktop version where the idea started *(Python, Tkinter)*

## About Me

- 🎓 B.A. Computer Science, Iona College (New York)
- 🧑‍🏫 English teacher at 212 English, Saitama (2015 to now), building learning tools for my own students
- 📈 Content creator with 400,000+ followers: managed analytics, growth and platform tools
- 🖥️ Background in IT support before moving to Japan
- 🗣️ English (native), Spanish, Japanese N4 (studying for JLPT N3)

## What I'm Looking For

I'm not looking to move to Japan. I'm already here, fully committed, and ready to contribute to a team. I'm looking for **junior backend, tools or iOS developer roles in Japan** (full-time).

## Connect

[![Email](https://img.shields.io/badge/-Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:oo0speed0oo@hotmail.com)

---

> "I build tools to solve my own problems, then share them."
