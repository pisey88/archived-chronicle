# 📜 Archived Chronicle

> *"Every day in history has a story. What's yours?"*

Archived Chronicle is an interactive web application that transforms any date into a rich historical journey. Whether you're curious about what happened on your birthday, a student researching history, or just someone who loves learning — Archived Chronicle brings the past to life.

---

## 🌍 Live Demo

🔗 [View Project](https://github.com/pisey88/archived-chronicle)

---

## 📖 About The Project

Most people scroll through their calendar without realizing that every single day is loaded with incredible moments from world history. Archived Chronicle changes that.

Pick any date. Instantly discover the wars that started, the legends that were born, the inventions that changed the world, and the moments that shaped humanity — all on that exact day throughout history.

This project was built as a Final Project for **INFO 251 – Web Development II** at **[Your School Name]**, Spring 2026.

---

## ✨ Features

### 🗓️ Today in History
Automatically loads 3–5 major historical events from today's date the moment you open the app. No setup needed — history greets you instantly.

### ⏳ Time Travel Date Picker
Enter any date you want and instantly travel back in time to see what happened on that exact day across all of recorded history.

### 🔽 Event Type Filter
Switch between different categories of historical records:
- 📌 **Events** — Major world events and milestones
- 🎂 **Births** — Famous people born on that day
- 💀 **Deaths** — Notable figures who passed on that day
- 🎉 **Holidays** — Observances and celebrations worldwide

### ⭐ Favorites System
Found something fascinating? Save it! Your favorite historical events are stored in your browser so they're always there when you come back.

### 🎲 Random Fact Cards
Hit the shuffle button and discover a completely random historical fact from any date in history. Great for learning something new every day.

### 🔍 Keyword Search
Search through the loaded events by typing any keyword — a name, a place, a topic — and instantly filter the results.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Structure | HTML5 (semantic elements) |
| Styling | CSS3 + Bootstrap 5 |
| Logic | Vanilla JavaScript (ES6+) |
| Data | Wikimedia "On This Day" REST API |
| Storage | Browser `localStorage` |

> ⚠️ Built with **zero JavaScript frameworks** — no React, no Vue, no Angular. Pure vanilla JS as required by course guidelines.

---

## 📁 Project Structure
archived-chronicle/
│
├── index.html              # Main HTML page (semantic structure)
├── styles.css              # All custom styles and CSS variables
├── README.md               # Project documentation
│
├── assets/
│   ├── book-open-svgrepo-com.svg     # Book icon
│   ├── calender-svgrepo-com.svg      # Calendar icon
│   └── shuffle-svgrepo-com.svg       # Shuffle icon
│
├── api.js                  # Handles all API fetch requests & error handling
└── app.js                  # Main JavaScript logic, DOM manipulation & events

---

## 🌐 API Used

**Wikimedia "On This Day" API** — Free, public, no API key required.
GET https://en.wikipedia.org/api/rest_v1/feed/v1/wikipedia/en/onthisday/{type}/{MM}/{DD}

| Parameter | Options |
|-----------|---------|
| `type` | `events` `births` `deaths` `holidays` `all` |
| `MM` | Month — e.g. `05` for May |
| `DD` | Day — e.g. `13` for the 13th |

**Example Request:**
GET https://en.wikipedia.org/api/rest_v1/feed/v1/wikipedia/en/onthisday/events/05/13

Returns a list of historical events that occurred on May 13th across all years in history.

---

## ⚙️ Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Edge)
- VS Code + Live Server extension *(recommended)*

### Run Locally

1. **Clone the repository**
```bash
git clone https://github.com/pisey88/archived-chronicle.git
```

2. **Open the project folder**
```bash
cd archived-chronicle
```

3. **Launch the app**
   - Right-click `index.html` in VS Code → **Open with Live Server**
   - Or simply open `index.html` directly in your browser

No installs. No build steps. Just open and go.

---

## 📌 Course Information

| | |
|-|-|
| **Course** | INFO 251 – Web Development II |
| **Semester** | Spring 2026 |
| **Project Type** | Final Project |
| **School** | [Your School Name] |

---

## 📄 License

This project was created for educational purposes as part of a university course. All historical data is sourced from Wikipedia via the Wikimedia REST API.