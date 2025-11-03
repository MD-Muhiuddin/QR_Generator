# QR Code Generator CLI 

This project is a simple **Command Line Interface (CLI)** QR Code Generator written in **Python**. It reads URLs (or any text) from a `.txt` file and generates corresponding QR Code images.

---

## 🧾 Features

- Reads URLs or text from a file (every even line).
- Uses the following line as the **output filename** (every odd line).
- Saves all QR images in a directory (default: `QrCode_outputImages`).
- Automatically creates the directory if it doesn't exist.
- Uses the built-in `qrcode` library.

---

## 📂 Files

| File Name         | Description                                      |
|-------------------|--------------------------------------------------|
| `QrGenProject.py` | Main script to read text and generate QR codes   |
| `qrRequirements.txt` | Input file: alternating lines of text & filenames |
| `README.md`       | Project description and usage instructions       |

---

## 📥 Example Input File (`qrRequirements.txt`)

```
https://youtube.com
youtube.png
https://facebook.com
facebook.png
https://google.com
google.png
```

---

## 🧪 How It Works

```python
gen_qr_from_file("qrRequirements.txt")
```

You can optionally specify a folder:

```python
gen_qr_from_file("qrRequirements.txt", "MyQrFolder")
```

If no folder is specified, `QrCode_outputImages` will be used.

---

## 🛠️ Setup Instructions

### 1. Install the required package

```bash
pip install qrcode[pil]
```

Or simply:

```bash
pip install qrcode
```

### 2. Run the script

```bash
python QrGenProject.py
```

---

## ✅ Output

All generated QR images will be saved in the specified folder.

---

## 👨‍💻 Author

- Developed by MD Muhiuddin
