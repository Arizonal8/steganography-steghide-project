
# 🔐 Steganography with Steghide (Kali Linux)

This project demonstrates how to hide and extract secret messages using the `steghide` tool in Kali Linux. It is designed for beginners in cybersecurity looking to understand steganography in a practical way.

---

## 📂 Project Features

- Hide a secret text file inside a JPEG image using Steghide
- Extract the hidden file using a passphrase
- Includes screenshots and step-by-step documentation
- Beginner-friendly project structure for GitHub

---

## 🛠️ Tools Used

- 🐧 Kali Linux
- 🧰 Steghide
- 🖼️ JPEG image as cover file
- 📝 Text file with secret message
- 📸 Screenshots of each step

---

## 📥 Embedding a Secret File

```bash
# Step 1: Create your secret message
echo "The eagle flies at midnight..." > secret.txt

# Step 2: Embed it in a cover image
steghide embed -cf Cover.jpg -ef secret.txt
```

You will be prompted to set a passphrase.

---

## 📤 Extracting the Secret File

```bash
steghide extract -sf Cover.jpg
```

Enter the same passphrase used during embedding to retrieve `secret.txt`.

---

## 📸 Screenshots

All steps are documented with screenshots stored in:

```
docs/screenshots/
```

---

## 📄 Full Documentation

Detailed explanation and step-by-step guide is in:

```
docs/project-report.md
```

---

## 📁 Project Structure

```
steghide-project/
├── README.md
├── requirements.txt
├── docs/
│   ├── project-report.md
│   └── screenshots/
├── secret.txt
├── Cover.jpg
└── embed_script.sh (optional)
```

---

## 👨‍💻 Author

**Ihekweme Arinze**  
Cybersecurity Enthusiast  
[GitHub Profile](https://github.com/Arizonal8)

---

## 📜 License

This project is licensed under the MIT License.
