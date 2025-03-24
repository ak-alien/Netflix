# Netflix Cookie Checker

This tool verifies the validity of Netflix cookies stored in `.txt` format and categorizes them based on subscription status. It is optimized for **Termux** and organizes valid, free, and invalid cookies into separate folders.

![NetflixSS](https://raw.githubusercontent.com/ak-alien/Netflix/refs/heads/main/src/Netflix.png)

## ✨ Features

- Checks Netflix cookies for active subscriptions.
- Extracts details like **subscription type, video quality, payment method, next payment date, and country**.
- Saves categorized cookies in respective directories (`Hits`, `Free`).
- Uses **multi-threading** for fast processing.

---

## 📥 Installation & Setup (Termux)

### 1️⃣ Install Required Packages

Ensure your Termux has the necessary dependencies:

```sh
pkg update && pkg upgrade -y
pkg install python -y
pip install requests bs4
```

### 2️⃣ Clone or Download the Script

Clone the repository:

```sh
git clone https://github.com/ak-alien/netflix.git
cd netflix
```

Alternatively, download `netflix.py` manually.

### 3️⃣ Place Cookies in the Correct Directory

Store your Netflix cookies (`.txt` format) in:

```
/sdcard/Netflix/Cookies/
```

The script will automatically read and process these files.

### 4️⃣ Run the Script

```sh
cd netflix
python netflix.py
```

---

## 📂 Output Directories

- **Valid Subscriptions** → `/sdcard/Netflix/Hits/`
- **Expired or No Subscription** → `/sdcard/Netflix/Free/`

---

## 🔎 Notes

- This tool **only** works with cookies in **Netscape format**.
- **Ensure Termux has storage permissions enabled**:

  ```sh
  termux-setup-storage
  ```

---

## ⚠️ Disclaimer

Use this tool responsibly. **Unauthorized access** to Netflix accounts **violates** their terms of service.
