### 💳 OmniKey Card Reader

A **Python-based** tool for reading **VISA** and **Mastercard** smart cards using the `pyscard` library. It detects a card, selects the appropriate application identifier (AID), and retrieves card details.

---

## 🚀 Features

- 📡 Detects and connects to a smart card automatically.
- 💳 Supports **VISA Debit** and **Mastercard** cards.
- 📥 Reads records and application data from the card.
- 🎨 Uses **colorized output** via `colorama` for better readability.
- 🔄 Handles APDU command transmission and response processing.

---

## 🛠️ Installation

Ensure you have Python **3.x** installed, then install dependencies:

```sh
pip install -r requirements.txt
```

### 📦 Required Dependencies:
- `pyscard` – Smart Card communication
- `pyasn1` & `pyasn1-modules` – ASN.1 encoding/decoding
- `colorama` – Colored terminal output

---

## 🔧 Usage

1. **Connect a Smart Card Reader** to your system.
2. **Insert a Smart Card** (VISA or Mastercard).
3. **Run the script**:

```sh
python smartcard_reader.py
```

---

## 📌 How It Works

1. **Detects** an inserted card.
2. **Selects AID** (e.g., `A0000000031010` for VISA).
3. **Reads and processes** available records.
4. **Prints extracted information** in a structured format.

Sample Output:

```
Card detected.
CARD TYPE : VISA DEBIT
Record #1
Application
    AID: ...
    Label: ...
...
```

---

## ⚠️ Known Issues

- Some cards may **not respond** to all APDU commands.
- Not all records contain **human-readable** data.
- Ensure your **smart card reader drivers** are installed.

---

## 📝 License

This project is **MIT licensed**.

---

### 💡 Contributions

Pull requests are **welcome**! If you'd like to contribute, feel free to **fork** the repo and submit a PR.

---

**📩 Need Help?** Open an issue on the **GitHub repository**! 🚀
