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
