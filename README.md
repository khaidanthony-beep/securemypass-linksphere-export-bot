# SecureMyPass CSV Export Bot (Selenium + LinkenSphere)

This project automates the SecureMyPass workflow using **Python Selenium** and **JavaScript injection**.  
It attaches to a running **LinkenSphere** profile via Chrome DevTools remote debugging, logs in, navigates to **My Links**, and clicks the **Export as CSV** button.

---

## ✨ Features
- Headful automation through **LinkenSphere**
- Smart **explicit waits** to handle slow UI loads
- **Robust export click**: finds button by text or XPath fallback
- **Multi-account support** via `.csv` input
- Environment-based secrets (`.env`) — no hardcoding credentials

---

## 📂 Project Structure

├─ main.py # Entry point
├─ scripts/
│ └─ export_click.js # JS helper for Export button
├─ data/
│ └─ accounts.csv # (optional) multiple username/passwords
├─ .env.example # Sample environment config
├─ requirements.txt
├─ .gitignore
└─ LICENSE

---

## ⚙️ Requirements
- Python 3.10+
- [LinkenSphere](https://sphere.tenebris.cc/) with remote debugging enabled
- Chromedriver (auto-managed with `webdriver-manager`)

---

## 🚀 Installation
```bash
git clone <YOUR_REPO_URL>
cd <YOUR_REPO_DIR>

# create & activate virtualenv
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
